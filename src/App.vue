<script>
import Header from './components/header/Header.vue';
import Main from './components/main/Main.vue';

export default {
    components: {
      Header,
      Main
    }
}
</script>

<template>
  <div class="container">
    <Header></Header>
    <Main></Main>
  </div>

</template>

<style>
  div.container {
    margin: 0 auto;
    max-width: 75rem;
    width: 80%;
  }
</style>
