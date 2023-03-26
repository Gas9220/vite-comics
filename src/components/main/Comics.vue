<script>
import ComicsList from './ComicsList.vue';

export default {
    name: 'Comics',
    components: {
        ComicsList
    }
}
</script>

<template>
    <section>
        <div class="container">
            <ComicsList></ComicsList>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

section {
    background-color: $bg-primary;
}

</style>