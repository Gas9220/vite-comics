<script>
import FooterTop from './FooterTop.vue';
import FooterLow from './FooterLow.vue';

export default {
    name: "Footer",
    components: {
        FooterTop,
        FooterLow
    }
}
</script>

<template>
    <footer>
        <FooterTop></FooterTop>
        <FooterLow></FooterLow>
    </footer>
</template>

<style lang="scss" scoped>

</style>