<template>
    <div class="contain">
        <ul>
            <li v-for="(item,index) in partners" :key="index" ><img :src="item.url" alt=""></li>
        </ul>
    </div>
</template>

<script>
     import {partners} from '../data/arrayPartners';
    export default {
        data() {
            return {
                partners: partners
            }
        },
    }
</script>

<style lang="scss" scoped>
    .contain{
        width: 1170px;
        margin: 2rem auto;
        ul{
            margin: 0;
            padding: 0;
            list-style: none;
            display: flex;
            justify-content: space-between;
            align-items: center;
            opacity: .5;
            filter: saturate(0);
        }
    }
</style>