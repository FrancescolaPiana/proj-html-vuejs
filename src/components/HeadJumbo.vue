<template>
    <div class="containe">
        <div class="text">
            <h6 class="sFont">i'm wingman</h6>
            <h1 class="pFont">Peace On Earth A Wonderfull Wish But No Way</h1>
            <p>Success isn't overnight. it's when everyday you get a alittle better than the day before. it all adds up</p>
            <a class="btn1" href="">Get Started For Free<i class="fa-solid fa-arrow-right-long"></i></a>
        </div>
        <div class="img">
        <img class="" src="/img/home-movation-hero-image.png" alt=""></div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .containe{
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 1170px;
            margin: 0 auto;
            padding: 2rem 0 ;
            .text{
                width: 35%;
                color: $cinder;
                margin-bottom: 50px;
                h6{
                    text-transform: uppercase;
                    margin-bottom: 1.5rem;
                }
                h1{
                    font-size: 3.3rem;
                    margin-bottom: 2rem;
                }
                p{
                    color: $courduray;
                    margin-bottom: 3rem;
                }
                a{
                    i{
                        margin-left: .4rem;
                    }
                }
            }
            .img{
                img{
                    transition: opacity 1s;
                }
            }
    }
</style>