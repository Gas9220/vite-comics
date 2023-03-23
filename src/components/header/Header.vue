<script>
import MainLogo from '../utility-view/MainLogo.vue';
import HeaderLinks from './HeaderLinks.vue';

export default {
    name: "Header",
    components: {
        MainLogo,
        HeaderLinks
    }
}
</script>

<template>
    <header>
        <MainLogo />
        <HeaderLinks />
    </header>
</template>

<style lang="scss">
header {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>