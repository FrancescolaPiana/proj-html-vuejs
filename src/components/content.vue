<template>
    <div class="content">
        <slot></slot>
        <div class="btn2">
            <a @click="back" class="back" ><i class="fa-solid fa-caret-up"></i></a>

            <span>1/4</span>

            <a @click="next" class="next" ><i class="fa-solid fa-caret-down"></i></a>
        </div>
    </div>
</template>

<script>
    export default {
        
        methods: {
            next(){
                this.$emit('next')
            },
            back(){
                this.$emit('back')
            },
            
        },
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;

    .content{
        width: 50%;
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
                text-decoration: none;
                transition: all 200ms;
                &:hover{
                    color: $logocolor;
                    transform: scale(2);
                    cursor: pointer;
                }
                i{
                    height: 20px;
                }
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
                text-decoration: none;
                transition: all 200ms;
                &:hover{
                    color: $logocolor;
                    transform: scale(2);
                    cursor: pointer;
                }
                i{
                    height: 20px;
                }
            }
    }
</style>