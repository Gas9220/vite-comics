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
div {
    padding: .625rem;

    h5 {
        color: white;
        width: 11.25rem;
        font-size: 1.125rem;
    }

    img {
        width: 100%;
        height: 11.25rem;
        object-fit: cover;
        padding: 0;
    }
}
</style>