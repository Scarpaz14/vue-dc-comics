<template>
  <div id="app">
    <HeaderComponent/>
    <MainComponent/>
    <FooterTopComponent/>
    <FooterMediumComponent/>
    <FooterBottomComponent/>
  </div>
</template>

<script>

import HeaderComponent from './components/blocks/HeaderComponent.vue';
import MainComponent from './components/blocks/MainComponent.vue';
import FooterTopComponent from './components/blocks/FooterTopComponent.vue';
import FooterMediumComponent from './components/blocks/FooterMediumComponent.vue';
import FooterBottomComponent from './components/blocks/FooterBottomComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterTopComponent,
    FooterMediumComponent,
    FooterBottomComponent,
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
