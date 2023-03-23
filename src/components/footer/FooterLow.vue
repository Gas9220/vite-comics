<script>
import FooterSocialIcons from './FooterSocialIcons.vue';

export default {
    name: "FooterLow",
    components: {
        FooterSocialIcons
    }
}
</script>

<template>
    <section>
        <div class="container">
            <a href="#">SIGN-UP NOW!</a>
            <FooterSocialIcons></FooterSocialIcons>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #303030;

    div.container {
        padding: 30px 0;

        display: flex;
        justify-content: space-between;
        align-items: center;

        a {
            display: inline-block;
            text-decoration: none;
            color: white;
            padding: 1.25rem;
            border: .1875rem solid #0782fa;

            &:hover {
                background-color: #0782fa;
                border: .1875rem solid white;
            }
        }

    }
}
</style>