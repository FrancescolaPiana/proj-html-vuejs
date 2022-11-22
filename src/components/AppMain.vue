<template>
  <div class="MainContainer">
    <MainNumbers/>
    <MainAboutMe/>
    <MainCourses/>
    <MainBookStore/>
    <Partners/>
    <Carousel/>
    <News/>
  </div>
</template>

<script>
import MainNumbers from './MainNumbers.vue';
import MainAboutMe from './MainAboutMe.vue';
import MainCourses from './/MainCourses.vue';
import MainBookStore from './/MainBookStore.vue';
import Partners from './/Partners.vue';
import Carousel from './/Carousel.vue';
import News from './/News.vue';
    export default {
        name: "AppHeader",
        components: {
          MainNumbers,
          MainAboutMe,
          MainCourses,
          MainBookStore,
          Partners,
          Carousel,
          News
          
        }
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;
    .MainContainer{

    }
</style>