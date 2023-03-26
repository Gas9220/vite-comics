<script>
export default {
    name: "ComicsItem",
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <section>
        <div>
            <img :src="image" :alt="title">
            <h5>{{ title }}</h5>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

div {
    color: white;
    cursor: pointer;
    align-self: top;
    padding: 20px;

    &:hover {
        color: $primary-color;
    }

    h5 {
        color: inherit;
        width: 11.25rem;
        font-size: 1.125rem;
    }

    img {
        width: 11.25rem;
        height: 11.25rem;
        object-fit: cover;
        padding: 0;

        &:hover {
        filter: grayscale(0.5);
    }
    }
}
</style>