<template>
    <main>
        <Albums/>
    </main>
</template>

<script>
import Albums from '../sections/Albums.vue'
export default {
    name: 'Main',
    components: {
        Albums
    }
}
</script>

<style lang="scss" scoped>
    main{
        background-color: #1e2d3b;
    }
</style>