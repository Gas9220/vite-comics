<script>
import Header from './components/header/Header.vue';
import Main from './components/main/Main.vue';
import Footer from './components/footer/Footer.vue';

export default {
    components: {
      Header,
      Main,
      Footer
    }
}
</script>

<template>
    <Header></Header>
    <Main></Main>
    <Footer></Footer>

</template>

<style lang="scss">
@use 'styles/global.scss' as *;
</style>
