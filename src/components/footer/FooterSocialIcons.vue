<script>
export default {
    name: "FooterSocial",
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
                <img :src="socialIcon.img" :alt="socialIcon.name">
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

        li {
            img {
                width: 3.125rem;

                &:hover {
                    cursor: pointer;
                    background-color: $primary-color;
                    border-radius: 50%;
                }
            }
        }
    }
}
</style>