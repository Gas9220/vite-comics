<script>
export default {
    name: "SocialIcon",
    props: {
        image: String,
        description: String
    }

}
</script>

<template>
    <img :src="image" :alt="description">
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

img {
    width: 3.125rem;

    &:hover {
        cursor: pointer;
        background-color: $primary-color;
        border-radius: 50%;
    }
}
</style>