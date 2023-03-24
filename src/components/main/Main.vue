<script>
import MainFeatures from './MainFeatures.vue';
import Comics from './Comics.vue';

export default {
    name: "Main",
    components: {
        MainFeatures,
        Comics
    }
}
</script>

<template>
    <main>
        <section class="jumbo">
        </section> 
        <Comics></Comics>
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