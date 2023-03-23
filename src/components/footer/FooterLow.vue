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
@use '../../styles/colors.scss' as *;

section {
    z-index: 13;
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
            border: .1875rem solid $primary-color;

            &:hover {
                background-color: $primary-color;
                border: .1875rem solid white;
            }
        }

    }
}
</style>