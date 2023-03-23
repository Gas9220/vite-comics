<script>
import MainFeatures from './MainFeatures.vue';
import NextFeatures from './NextFeatures.vue';

export default {
    name: "Main",
    components: {
        MainFeatures,
        NextFeatures
    }
}
</script>

<template>
    <main>
        <NextFeatures></NextFeatures>
        <MainFeatures></MainFeatures>
    </main>
</template>

<style lang="scss">
</style>