<template>
   <div class="special-link">
       <div class="container">
            <div class="image-special-link">
                <img src="../assets/image/buy-comics-digital-comics.png" alt="">
                <h3>Digital comics</h3>
            </div>
            <div class="image-special-link">
                <img src="../assets/image/buy-comics-digital-comics.png" alt="">
                <h3>Digital comics</h3>
            </div>
             <div class="image-special-link">
                <img src="../assets/image/buy-comics-digital-comics.png" alt="">
                <h3>Digital comics</h3>
            </div>
             <div class="image-special-link">
                <img src="../assets/image/buy-comics-digital-comics.png" alt="">
                <h3>Digital comics</h3>
            </div>
             <div class="image-special-link">
                <img src="../assets/image/buy-comics-digital-comics.png" alt="">
                <h3>Digital comics</h3>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SecondMainComponent'

}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

.special-link{
    background-color: var(--primary-color);
    padding: 3.125rem;
    color: white;

    & .container{
        display: flex;
        justify-content: center;
    }

    .image-special-link {
        @include imageflex
    }

    & img{
        width: 4.375rem;
        margin-right: 0.625rem;
    }
}

</style>