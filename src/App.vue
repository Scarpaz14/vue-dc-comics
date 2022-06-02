<template>
  <div id="app">
    <HeaderComponent/>
    <MainComponent/>
    <SecondMainComponent/>
    <FooterTopComponent/>
    <FooterBottomComponent/>
  </div>
</template>

<script>

import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import SecondMainComponent from './components/SecondMainComponent.vue';
import FooterTopComponent from './components/FooterTopComponent.vue';
import FooterBottomComponent from './components/FooterBottomComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    SecondMainComponent,
    FooterTopComponent,
    FooterBottomComponent,
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
