<template>
    <main>
        <HeroSection/>
    </main>
</template>

<script>
import HeroSection from '../sections/HeroSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection
    }
}
</script>

<style lang="scss" scoped>

main{
    background-color: black;
}


</style>