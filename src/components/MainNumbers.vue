<template>
    <div class="containe">
        <ul>
            <li class="sFont">
                <div id="saro" class="numbers">{{valueContainer1}}</div>
                <div class="text">finished sessions</div>
            </li>
            <li class="sFont">
                <div class="numbers">{{valueContainer2}}%</div>
                <div class="text">satisfaction rate</div>
            </li>
            <li class="sFont">
                <div class="numbers">{{valueContainer3}}+</div>
                <div class="text">enrolled leaners</div>
            </li>
            <li class="sFont">
                <div class="numbers">{{valueContainer4}}</div>
                <div class="text">online instructors</div>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
    data() {
        return {
            valueContainer1: 0,
            valueContainer2: 0,
            valueContainer3: 0,
            valueContainer4: 0,
        }
        
    },
    methods: {
        numberGrowing1(){
                let value = document.getElementById('saro')
                console.log(document.getElementById('saro'));

                let progressEndValue = 1926;
                let speed = 1 * 10^-9999999 ;

                let progress = setInterval(() => {
                    if (this.valueContainer1 < progressEndValue){
                        this.valueContainer1 ++;
                        this.valueContainer1 ++;
                        this.valueContainer1 ++;
                        this.valueContainer1 ++;
                        this.valueContainer1 ++;
                        this.valueContainer1 ++;
                    }
                    else{
                        clearInterval(progress);
                    }
                    }, speed)
                },
                numberGrowing2(){
                let value = document.getElementById('saro')
                console.log(document.getElementById('saro'));

                let progressEndValue = 100;
                let speed = 10 ;

                let progress = setInterval(() => {
                    if (this.valueContainer2 < progressEndValue){
                        this.valueContainer2 ++;
                    }
                    else{
                        clearInterval(progress);
                    }
                    }, speed)
                },
                numberGrowing3(){
                let value = document.getElementById('saro')
                console.log(document.getElementById('saro'));

                let progressEndValue = 3092;
                let speed = 1 ;

                let progress = setInterval(() => {
                    if (this.valueContainer3 < progressEndValue){
                        this.valueContainer3 ++;
                        this.valueContainer3 ++;
                        this.valueContainer3 ++;
                        this.valueContainer3 ++;
                    }
                    else{
                        clearInterval(progress);
                    }
                    }, speed)
                },
                numberGrowing4(){
                let value = document.getElementById('saro')
                console.log(document.getElementById('saro'));

                let progressEndValue = 200;
                let speed = 1 ;

                let progress = setInterval(() => {
                    if (this.valueContainer4 < progressEndValue){
                        this.valueContainer4 ++;
                    }
                    else{
                        clearInterval(progress);
                    }
                    }, speed)
                },
            },

        created() {
           this.numberGrowing1();
           this.numberGrowing2();
           this.numberGrowing3();
           this.numberGrowing4();
        }
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