<template>
    <div class="containe">
        <a href="" class="logo">
            <img src="/img/dark-logo.png" alt="logo MaxCoach">
        </a>
        <div class="list">
            <ul>
                <li v-for="(element,i) in list" :key="i" ><a href="">{{element.listcontent}}<i class="fa-solid fa-angle-down"></i></a></li>
            </ul>
        </div>
        <div class="social">
            <ul>
                <li v-for="(item,index) in social" :key="index" ><a href=""><i :class="item.text"></i></a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    import {arrayList} from '../data/arrayList';
    import {socials} from '../data/arraySocials';
    export default {
        data() {
            return {
                list: arrayList,
                social: socials
            }
        },
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
        padding: 1rem 0 ;
        .logo{
            img{
                width: 45%;
            }
        }
        .list{
            ul{ 
                margin: 0;
                padding: 0;
                list-style: none;
                display: flex;
                gap: 1rem;
                li{
                    a{
                        color: $logocolor;
                        text-decoration: none;
                        font-weight: 500;

                        &:hover{
                            filter: brightness(1.8);
                        }
                        i{  
                            margin-left: .3rem;
                            font-size: .8rem;
                        }
                    }
                }
            }
        }
        .social{
            ul{ 
                margin: 0;
                padding: 0;
                list-style: none;
                display: flex;
                gap: 1rem;
                li{
                    a{
                        display: flex;
                        align-items: center;
                        color: $cinder;
                        text-decoration: none;
                        transition: all 500ms;
                        &:hover{
                            filter: brightness(2);
                            transform: scale(1.2);
                        }

                        &:hover i{
                            text-shadow: 2px 2px 0px rgba(0, 0, 0, 0.3);
                        }
                        i{  
                            font-size: 1.3rem;
                            margin-left: .3rem;
                            transition: all 500ms;
                        }
                    }
                }
            }
        }
    }
</style>