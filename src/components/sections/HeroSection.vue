<template>
    <section>
        <div class="content-container">
            <div class="hero-img">

            </div>
        </div>
    </section>
  
</template>

<script>
export default {
    name: 'HeroSection'
}
</script>

<style lang="scss" scoped>

.content-container{
    & h2{
        color:white
    }
}

.hero-img{
    background-image: url(../../assets/image/jumbotron.jpg);
    background-size: cover;
    width: 100%;
    min-height: 450px;
}

</style>