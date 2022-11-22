<template>
  <header>
    <AppHeader/>
  </header>
  <main>
    <AppMain/>
  </main>
  <footer>
    <AppFooter/>
  </footer>
</template>

<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  export default {
    components:{
      AppHeader,
      AppMain,
      AppFooter
    },
  }
</script>

<style lang="scss" scoped>
@use './styles/general.scss' as* ;

</style>