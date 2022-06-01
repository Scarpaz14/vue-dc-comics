<template>
  <div id="app">
    <HeaderComponent/>
    <MainComponent/>
    <SecondMainComponent/>
  </div>
</template>

<script>

import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import SecondMainComponent from './components/SecondMainComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    SecondMainComponent,
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
