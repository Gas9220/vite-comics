<script>

export default {
    name: 'Feature',
    props: {
        image: String,
        text: String
    }
}
</script>

<template>
    <div>
        <img :src="image" :alt="text">
        <h4>{{ text.toUpperCase() }}</h4>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

div {
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    padding: 2rem;
    height: 100%;

    h4 {
        font-size: .8125rem;
    }

    img {
        width: 3.125rem;
    }
}
</style>