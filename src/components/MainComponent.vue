<template>
    <main>
        <div class="container">
            <div class="content-container">
                <h2>-->Content goes here </h2>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: 'MainComponent'

}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

main{
    background-color: black;
    padding: 3.125rem;
}

.content-container{
    & h2{
        color:white
    }
}

</style>