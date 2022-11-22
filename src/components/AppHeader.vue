<template>
    <div class="HeaderContainer">
    <HeadBar/>
    <HeadJumbo/>
    <HeadFix/>
    </div>
</template>

<script>
import HeadBar from './HeadBar.vue';
import HeadJumbo from './HeadJumbo.vue';
import HeadFix from './HeadFix.vue';
    export default {
        name: "AppHeader",
        components: {
            HeadBar,
            HeadJumbo,
            HeadFix
        }
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .HeaderContainer{
        background-image: url(/img/background-pattern-wavify.png);
        background-color: $amour;
        height: 700px;
        overflow-y: hidden;
    }
</style>