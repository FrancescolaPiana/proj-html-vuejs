<template>
    <div class="contain">
        <div class="pretitle sFont">
            begin your journey at maxcoach
        </div>
        <div class="title pFont">
            latest  <span>online courses</span> 
        </div>
        <div class="courses">
            <div class="car" v-for="(item,i) in courslist" :key="i">
                <img class="img" :src="item.url" alt="">
                <div class="text">
                    <h3 class="unit mFont" >${{item.price.unit}}.<span class="cent">{{item.price.cent}}</span></h3>
                    <h5>{{item.title}}</h5>
                    <div>
                        <span class="lessons"><i class="fa-solid fa-file-invoice"></i>{{item.lessons}} Lessons</span>
                        <span class="students"><i class="fa-regular fa-user"></i>{{item.students}} Students</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="btn1"> View all courses <i class="fa-solid fa-arrow-right-long"></i></div>
    </div>
</template>

<script>
 import {courses} from '../data/arrayCourses';
 export default {
        data() {
            return {
                courslist: courses,
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '../styles/general.scss' as* ;
    .contain{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        width: 1170px;
        margin: 1rem auto;
        padding: 1rem 0 ;
        .pretitle{
            font-size: .8rem;
            text-align: center;
            text-transform: uppercase;
            letter-spacing: .1rem;
            font-weight: bold;
            color: $graychateau;
        }
        .title{
            color: $logocolor;
            margin: 1.5rem auto;
            font-size: 2.8rem;
            text-align: center;
            letter-spacing: .1rem;
            text-transform: capitalize;
            span{
                color: $mountainmeadown;
            }
        }
        .courses{
            width: 1170px;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            .car{
                margin-top: 1.5rem;
                width: 360px;
                border-radius: .3rem;
                transition: all 250ms;
                &:hover{
                    background-color: $athensgray;
                    cursor: pointer;
                    box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.3);
                }
                .img{
                    width: 360px;
                    box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.3);
                }
                div{
                    padding: 1rem 2rem;
                    h3{
                    font-weight: bold;
                    color: $mountainmeadown;
                    font-size: 1.5rem;
                        span{
                        font-size: 1rem;
                        }
                    }
                    h5{
                        text-transform: capitalize;
                        font-size: 1.1rem;
                        line-height: 1.8;
                        color: $logocolor;
                        font-weight: bold;
                    }
                    div{
                        display: flex;
                        justify-content: space-between;
                        .lessons{
                            white-space: nowrap;
                            max-width: 48%;
                            overflow-x: hidden;
                            text-overflow: ellipsis;
                            i{
                                margin-right: .3rem;
                            }
                        }
                        .students{
                            white-space: nowrap;
                            max-width: 48%;
                            overflow: hidden;                            
                            text-overflow: ellipsis;
                        }
                    }
                }
            }
        }
        .btn1{
                margin-top: 3rem;
                padding: .8rem 4.5rem;
                display: flex;
                align-items: center;
                gap: .3rem;
                box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.3);
            }
    }
</style>