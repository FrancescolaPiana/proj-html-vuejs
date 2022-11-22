<template>
    <div class="containe">
        <ul>
            <li v-for="(id,ina) in val" :key="ina" ><a href=""><i :class="id.text"></i></a></li>
        </ul>
    </div>
</template>

<script>
    import {icons} from '../data/arrayIcons';
    export default {
        data() {
            return {
            val: icons
        
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '../styles/general.scss' as* ;
    .containe{
        display: flex;
        position: fixed;
        top: 10rem;
        right: 0;
        ul{ 
                margin: 0;
                padding: 0;
                list-style: none;
                display: flex;
                justify-content: center;
                flex-direction: column;
                background-color: $white;
                gap: .3rem;
                border-radius: .3rem;
                box-shadow: -2px 2px 5px rgba(0, 0, 0, 0.3);
                li{
                    display: flex;
                    justify-content: center;
                    a{
                        margin: 0;
                        color: $logocolor;
                        text-decoration: none;
                        padding: .4rem .6rem;
                        font-weight: 500;

                        &:hover{
                            filter: brightness(0);
                            text-shadow: 2px 2px 2px rgba(0, 0, 0, .5);
                        }
                        i{  
                            font-size: 1.2rem;
                        }
                    }
                }
            }
    }
</style>