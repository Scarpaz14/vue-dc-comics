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

import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterTopComponent from './components/FooterTopComponent.vue';
import FooterMediumComponent from './components/FooterMediumComponent.vue';
import FooterBottomComponent from './components/FooterBottomComponent.vue';
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
