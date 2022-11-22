<template>
    <div class="contain">
        <div class="subtitle sFont">
            blog updated
        </div>
        <div class="title pFont">
            Intresting <span>article updated</span> daily
        </div>
        <div class="news">
            <div class="car" v-for="(item,i) in newslist" :key="i">
                <img class="img" :src="item.url" alt="">
                <div class="text">
                    <div>
                        <span class="date"><i class="fa-solid fa-file-invoice"></i>{{item.lessons}} Lessons</span>
                    </div>
                    <h5>{{item.title}}</h5>
                    <div>
                        <span class="description"><i class="fa-regular fa-user"></i>{{item.students}} Students</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import {news} from '../data/arrayNews';
    export default {
        data() {
            return {
                newslist: news
            }
        },
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .contain{
        width: 1170px;
        margin: 0 auto;
        .subtitle{
            text-transform: uppercase;
            font-weight: 600;
            color: $courduray;
        }
        .title{
            font-size: 3rem;
            span{
                color: $mountainmeadown;
            }
        }
        
    }
</style>