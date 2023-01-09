<script>
import HeaderDc from './components/HeaderDc.vue';
import MainDc from './components/MainDc.vue';
import FooterDc from './components/FooterDc.vue';

export default {

  components: {
    HeaderDc,
    MainDc,
    FooterDc
  }
}
</script>

<template>
  <header>
    <HeaderDc />
  </header>

  <main>
    <MainDc />
  </main>

  <footer>
    <FooterDc />
  </footer>
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
