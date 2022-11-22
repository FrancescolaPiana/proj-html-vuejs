<template>
  <div class="MainContainer">
    <MainNumbers/>
    <MainAboutMe/>
    </div>
</template>

<script>
import MainNumbers from './MainNumbers.vue';
import MainAboutMe from './MainAboutMe.vue';
    export default {
        name: "AppHeader",
        components: {
          MainNumbers,
          MainAboutMe,
          
        }
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .MainContainer{

    }
</style>