<template>
    <div class="containe">
        <div class="content">
            <ul class="address">
            <h5>Address</h5>
                <li>382 NE 191st ST # 87394 Miami, FL 33197-3899</li>
                <li>+1(305) 547-9909(9am -5pm EST, Monday - Friday)</li>
                <li>support@maxcoach.com</li>
                <li>
                    <a v-for="(item,index) in social" :key="index" href=""><i :class="item.text"></i></a>
                </li>
            </ul>
            <div class="links">
                <ul> <h5>Explore</h5>
                    <li><a href="">Start here</a></li>
                    <li><a href="">Blog</a></li>
                    <li><a href="">About us</a></li>
                </ul>
                <ul> <h5><br></h5>
                    <li><a href="">Success story</a></li>
                    <li><a href="">Courses</a></li>
                    <li><a href="">Contact us</a></li>
                </ul>
                <ul> <h5>Information</h5>
                    <li><a href="">Membership</a></li>
                    <li><a href="">Purchase guide</a></li>
                    <li><a href="">Privacy policy</a></li>
                    <li><a href="">Term of service</a></li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            <span> &copy; 2020 Maxcoach. All Rights Reserved</span>
        </div>
    </div>
</template>

<script>
import {socials} from '../data/arraySocials';
    export default {
        data() {
            return {
                social: socials
            }
        },
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .containe{
        width: 100%;
        background-color: $cinder;
        .content{
            width: 1170px;
            margin: 0 auto;
            padding: 3rem 0;
            display: flex;
            justify-content: space-between;
            ul{
                color: $white;
                padding: 0;
                margin: 0;
                list-style: none;
                h5{
                    font-weight: 600;
                    margin-bottom: 1.8rem;
                }
                li{
                    color: $silversand;
                    font-size: .9rem;
                    display: flex;
                    gap: 1.5rem;
                    margin-top: .8rem;
                    a{
                        color: $silversand;
                        text-decoration: none;
                        font-size: 1rem;

                        &:hover{
                            filter: brightness(1.5);
                        }
                    }
                }
            }
            div{
                display: flex;
                gap: 3rem;
                ul{
                color: $white;
                padding: 0;
                margin: 0;
                list-style: none;
                h5{
                    font-weight: 600;
                }
                li{
                    color: $silversand;
                    font-size: .9rem;
                    display: flex;
                    gap: 1.5rem;
                    margin-top: .8rem;
                        a{
                            font-weight: 600;
                            color: $silversand;
                            text-decoration: none;
                            font-size: 1rem;
                            &:hover{
                            filter: brightness(1.5);
                            }
                        }
                    }
                }
            }
        }
        .copyright{
            display: flex;
            justify-content: center;
            padding-bottom: 3rem;
            span{
                font-size: .8rem;
                color: $silversand;
            }
        }
    }
</style>