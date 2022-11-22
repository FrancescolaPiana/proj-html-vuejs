<template>
<div class="all">
    <div class="subtitle">
        <span class="sFont">about me</span>
    </div>
    <div class="containe1">
        <h1 class="pFont" >how to be an alpha male: the 15 habits of true alphas</h1>
        <div class="sideText">
            <div class="mText"
            >Want to learn how to be <span>an alpha male</span>? How to be more masculine?
            How to be the man you've always wanted to be?
            </div>
            
            <div class="sText">
            Your goal is to show the consistency of business, core values, and customer care.
            Punctuality, responsibility, individuality, accuracy, enthusiasm you have to clearly 
            explain how these qualities are applicable to your work. And the important thing is you do love what you do.
            </div>
        </div>
    </div>
    <div class="containe2">
        <div class="img">
            <img class="" src="/img/icon-youtube-play.png" alt="">
        </div>
        <div class="text">
            <p class="pFont">
                "Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."
            </p>
            <img src="/img/home-movation-shape-01.png" alt="">
            <h5>Kaixa Stark</h5>
            <span class="sFont">wingman</span>
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
.all{
    width: 1170px;
    margin: 2rem auto;
    padding: 1rem 0 ;
    .subtitle{
        text-transform: uppercase;
        color: $mountainmeadown;
        margin-bottom: 1.8rem;
    }
    .containe1{
        display: flex;
        h1{
            text-transform: capitalize;
            padding-right: 10rem;
            width: 50%;
            margin: 0;
            line-height: 1.3;
        }
        .sideText{
            width: 50%;
            .mText{
                font-size: 1.1rem;
                margin-bottom: 1rem;
                font-weight: 500;
                span{
                    color: $mountainmeadown;
                }
            }
            .sText{
                font-size: .96rem;
                color: $graychateau;
            }
        }
    }
    .containe2{
        margin: 8rem auto;
        display: flex;
        justify-content: space-between;
        .img{
            background-image: url(/img/home-movation-video-poster-670x450.jpg);
            width: 670px;
            height: 450px;
            border-radius: .3rem;
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0px 3px 10px rgba(0, 0, 0, 0.3);
        }
        .text{
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            width: 40%;
            padding: 4rem 3rem;
                p{
                font-size: 1.5rem;
                line-height: 1.6;
                }
                img{
                    margin-top: 5rem;
                }
                h5{
                    margin-top: 1.5rem;
                }
                span{
                    font-size: .8rem;
                    text-transform: uppercase;
                    color: $silversand;
                }
            
        }
    }
}
</style>