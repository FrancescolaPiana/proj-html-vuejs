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
                        <span class="date sFont"><i class="fa-solid fa-calendar"></i>{{item.date}}</span>
                    </div>
                    <h5>{{item.title}}</h5>
                    <div>
                        <span class="description">{{item.description}}</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="btn">
            <a class="sFont" href="">view all posts</a>
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
        margin-bottom: 10rem,;
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
        .news{
                margin-top: 2.6rem;
                display: flex;
                justify-content: space-between;
            .car{
                width: 280px;
                .img{
                    width: 280px;
                    border-radius: .3rem;
                }
                .text{
                    padding: 2rem 0;
                    width: 280px;
                    overflow: hidden;
                    div{
                        margin-bottom: 1rem;
                        .date{
                            color: $courduray;
                            i{
                                margin-right: .3rem;
                            }
                        }
                    }
                    .h5{

                    }
                    div{
                        margin-bottom: 1rem;
                        .description{
                            font-size: .9rem;
                            color: $courduray;
                        }
                    }
                }
        }
        }
        .btn{
            display: flex;
            justify-content: center;
            a{
                text-align: center;
                text-transform: uppercase;
                text-underline-offset: .5rem;
                color: $mountainmeadown;
                font-weight: 600;
                opacity: .7;
            }
        }
    }
</style>