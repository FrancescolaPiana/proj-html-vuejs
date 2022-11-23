<template>
    <div class="containe">
        <content  @next='next' @back='back'>
           
            <carous class="story" v-for="(item,index) in arrayRealStories" 
            :key="item" 
            :index="index"
            :visibleSlide="visibleSlide"
            >
                <h5 class="sFont mn">real stories</h5>
                <p class="sFont">{{item.text}}</p>
                <img :src="item.url" alt="">
                <h5>{{item.name}}</h5>
                <span>/ {{item.occupation}}</span>
            </carous>
        </content>
        
        <div class="image">
            <img src="/img/home-movation-testimonial-image.jpg" alt="">
        </div>

    </div>
</template>

<script>
import carous from '../components/carous.vue'
import content from '../components/content.vue'
import {stories} from '../data/arrayRealStories';
    export default {
        data() {
            return {
                arrayRealStories: stories,
                visibleSlide : 0,
            }
        },
        computed: {
            storiesLen(){
                return this.arrayRealStories.length;
            }
        },

        methods: {
            next(){
                if (this.visibleSlide >= this.storiesLen - 1) {
                    this.visibleSlide = 0;
                }else{
                    this.visibleSlide++;
                }
            },

            back(){
                if (this.visibleSlide <= 0) {
                    this.visibleSlide =  this.storiesLen - 1;
                }else{
                    this.visibleSlide--;
                }
            }
        },
        components: {
            content,
            carous
        },

    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .containe{
        position: relative;
        margin: 6rem 0;
        width: 100%;
        display: flex;
        .story{
            height: 100%;
            background-image: url(/img/background-pattern-wavify.png);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            margin: 0;
            .mn{
                color: $mountainmeadown;
                text-transform: uppercase;
                font-size: .9rem;
                font-weight: bold;
                letter-spacing: .1rem;
            }
            p{
                padding-top: 1.8rem;
                padding-bottom: 1rem;
                text-align: center;
                width: 45%;
                font-size: 1.5rem;
            }
            img{
                border-radius: 100%;
                width: 15%;
                margin-bottom: 2rem;
            }
            h5{
                text-transform: capitalize;
                color: cinder;
            }
            span{
                color: $silversand;
                text-transform: capitalize;
            }
        }

        .image{
            width: 50%;
            img{
                width: 100%;
            }
        }
    }
</style>