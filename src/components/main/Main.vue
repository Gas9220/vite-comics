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
        <section class="jumbo">
        </section> 
        <NextFeatures></NextFeatures>
        <MainFeatures></MainFeatures>
    </main>
</template>

<style lang="scss" scoped>
main {
    section.jumbo {
        background-image: url('/jumbotron.jpg');
        height: 25rem;
        background-repeat: no-repeat;
        background-size: cover;
    }
}
</style>