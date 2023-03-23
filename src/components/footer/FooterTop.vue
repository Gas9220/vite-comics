<script>
import FooterLinks from './FooterLinks.vue';

export default {
    name: "FooterTop",
    components: {
        FooterLinks
    }
}
</script>

<template>
<div class="footer-top">
    <div class="container">
        <FooterLinks></FooterLinks>

        <img src="/dc-logo-bg.png" alt="logo">
    </div>
</div>
</template>

<style lang="scss" scoped>
.footer-top {
    overflow: hidden;
    background-image: url('/footer-bg.jpg');

    div {
        position: relative;

        img {
           width: 400px;
           position: absolute;
           right: 0;
           top: -50px;
        }
    }
}
</style>