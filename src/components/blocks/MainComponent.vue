<template>
    <main>
        <HeroSection/>
        <SeriesSection/>
    </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue'
import SeriesSection from '../sections/SeriesSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection,
        SeriesSection,
    },
   
}
</script>

<style lang="scss" scoped>

main{
    background-color: black;
}


</style>