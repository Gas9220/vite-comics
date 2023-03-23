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
    </div>
</div>
</template>

<style lang="scss" scoped>
.footer-top {
    background-image: url('/footer-bg.jpg');
}
</style>