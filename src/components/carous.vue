<template>
    <div v-show="visibleSlide === index" class="carous-slide">
        <slot></slot>
    </div>
</template>

<script>
    export default {
        props: ['visibleSlide','index']
    }
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as* ;

.carous-slide{
}
</style>