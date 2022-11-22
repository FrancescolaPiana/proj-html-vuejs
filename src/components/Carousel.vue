<template>
    <div class="containe">
        <div class="story">
            <h5 class="sFont mn">real stories</h5>
            <p class="sFont">i am free to learn at my own pace, follow my own schedule and chose the subject i want to learn from the syllabus. Great study portal for people like me.</p>
            <img src="/img/testimonial-avata-02.jpg" alt="">
            <h5>mina hollace</h5>
            <span>/ freelancer</span>
        </div>
        <div class="btn2">
            <a class="back" href=""><i class="fa-solid fa-caret-up"></i></a>
            <span>1/4</span>
            <a class="next" href=""><i class="fa-solid fa-caret-down"></i></a>
        </div>
        <div class="image">
            <img src="/img/home-movation-testimonial-image.jpg" alt="">
        </div>

    </div>
</template>

<script>
    export default {
        
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
            width: 50%;
            background-image: url(/img/background-pattern-wavify.png);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
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
                border-radius: 50%;
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
        .btn2{
            position: absolute;
            left: 892px;
            top: 42%;
            background-color: $white;
            width: 120px;
            height: 120px;
            border-radius: 50%;
            box-shadow: 0px 3px 5px rgba(0, 0, 0, 0.3);
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-direction: column;
            overflow: hidden;
            .back{
                height: 40px;
                width: 130px;
                border-radius: 100px 100px 0px 0px;
                text-align: center;
                color: $silversand;
                display: flex;
                justify-content: center;
                align-items: center;
                i{
                    height: 20px;
                }
            }
            .next{
                display: flex;
                justify-content: center;
                color: $silversand;
                text-align: center;
                height: 40px;
                width: 130px;
                border-radius:  0px 0px 100px 100px;
                align-items: center;
                i{
                    height: 20px;
                }
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