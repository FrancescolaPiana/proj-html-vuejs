<template>
    <div class="containe">
        <ul>
            <li class="sFont">
                <div class="numbers">1.926</div>
                <div class="text">finished sessions</div>
            </li>
            <li class="sFont">
                <div class="numbers">100%</div>
                <div class="text">satisfaction rate</div>
            </li>
            <li class="sFont">
                <div class="numbers">3092+</div>
                <div class="text">enrolled leaners</div>
            </li>
            <li class="sFont">
                <div class="numbers">200</div>
                <div class="text">online instructors</div>
            </li>
        </ul>
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
        margin: 2rem auto;
        padding: 1rem 0 ;
        ul{ 
                margin: 0;
                padding: 0;
                list-style: none;
                display: flex;
                gap: 1rem;
                li{
                    background-image: url(/img/background-pattern-grid-line-06.png);
                    background-repeat: no-repeat;
                    padding: 1rem 2.5rem;
                    div{
                        display: flex;
                        justify-content: center;
                    }
                    .numbers{
                            font-size: 2.2rem;
                            font-weight: bold;
                            color: $mountainmeadown;
                            margin-bottom: 1rem;
                        }
                    .text{
                        font-size: .9rem;
                        text-transform: uppercase;
                        font-weight: bold;
                        letter-spacing: .2rem;
                    }
                }
        }
    }
</style>