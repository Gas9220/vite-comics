<script>
import SocialIcon from '../utility-view/SocialIcon.vue';

export default {
    name: "FooterSocial",
    components: {
        SocialIcon
    },
    data() {
        return {
            socialIcons: [
                {
                    name: "Facebook",
                    img: '/social-icons/footer-facebook.png'
                },
                {
                    name: "Twitter",
                    img: '/social-icons/footer-twitter.png'
                },
                {
                    name: "Facebook",
                    img: '/social-icons/footer-youtube.png'
                },
                {
                    name: "Facebook",
                    img: '/social-icons/footer-pinterest.png'
                },
                {
                    name: "Facebook",
                    img: '/social-icons/footer-periscope.png'
                },
            ]
        }
    }
}
</script>

<template>
    <div>
        <h4>FOLLOW US</h4>
        <ul>
            <li v-for="socialIcon in socialIcons">
                <SocialIcon :image="socialIcon.img" :description="socialIcon.name"></SocialIcon>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

div {
    display: flex;
    align-items: center;

    h4 {
        color: $primary-color;
        font-size: 1.125rem;
        margin-right: .625rem;
        cursor: pointer;
    }

    ul {
        display: flex;
        list-style-type: none;
    }
}
</style>