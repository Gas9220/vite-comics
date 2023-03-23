<script>
import MainFeatures from './MainFeatures.vue';

export default {
    name: "Main",
    components: {
        MainFeatures
    }
}
</script>

<template>
    <main>
        <div class="next-step">
            <h1> ---- Content Goes here -----</h1>
        </div>
        <MainFeatures></MainFeatures>
    </main>
</template>

<style lang="scss">
main {
    div.next-step {
        background-color: black;
        padding: 1.875rem;

        h1 {
            color: white;
        }

    }
}
</style>