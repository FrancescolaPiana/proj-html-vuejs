<template>
<div class="contain">
    <div class="contain2">
        <div class="title">
            book store online
        </div>
        <div class="text">
            <h1 class="pFont ">be alpha with <span>wingman's book</span></h1>
            <ul class="fa-ul">
                <li><span class="fa-li"><i class="fa-solid fa-check"></i></span>Help yoy undestans yourselfe better</li>
                <li><span class="fa-li"><i class="fa-solid fa-check"></i></span>Revealing mature tips</li>
                <li><span class="fa-li"><i class="fa-solid fa-check"></i></span>Give the eight advice</li>
                <li><span class="fa-li"><i class="fa-solid fa-check"></i></span>Fascinating examples of alpha man</li>
            </ul>
        </div>
        <div>
            <span class="btn1">get free ebook</span>
        </div>
    </div>
    <div class="cards">
        <div class="car">
                <img src="/img/product-book-11-400x400.jpg" alt="">
                <h5>alpha man by maxcoach</h5>
                <h3>$29.<span>00</span> </h3>
        </div>
        <div class="car">
                <img src="/img/product-book-10-400x400.jpg" alt="">
                <h5>real man 4.0 by maxcoach</h5>
                <h3>$39.<span>00</span> </h3>
        </div>
    </div>
</div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .contain{
        width: 1170px;
        margin: 5rem auto 8rem auto;
        display: flex;
        justify-content: space-between;
        .contain2{
            width: 30%;
            .title{
            margin-top: 0;
            text-transform: uppercase;
            letter-spacing: .1rem;
            font-weight: bold;
            color: $courduray;
            margin-bottom: .7rem;
        }
            .text{
                h1{
                    color: $logocolor;
                    text-transform: capitalize;
                    line-height: 1.5;
                    span{
                        color: $mountainmeadown;
                    }
                }
                ul{ 
                    margin-left: 1.4rem;
                    margin-bottom: 2rem;
                    li{
                        margin-bottom: .3rem;
                        .fa-check{
                            color: $mountainmeadown;
                        }
                    }
                }
            }
            div{
                    margin-top: 2rem;
                    span{
                        display: inline-block;
                        
                    }
                }
        }
        .cards{
            width: 60%;
            display: flex;
            justify-content: space-between;
            div{
                img{
                    width: 19rem;
                }
                h3{
                    margin-bottom: 0;
                    text-align: center;
                    font-weight: bold;
                    color: $mountainmeadown;
                    font-size: 1.5rem;
                        span{
                        font-size: 1rem;
                        }
                    }
                    h5{
                        margin-top: .8rem;
                        text-align: center;
                        text-transform: capitalize;
                        font-size: 1.1rem;
                        line-height: 1.8;
                        color: $logocolor;
                        font-weight: bold;
                    }
            }
        }
    }
</style>