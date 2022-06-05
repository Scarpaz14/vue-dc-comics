<template>
   <div class="special-link">
       <div class="container">
            <div class="image-special-link" v-for="(img, index) in images" :key="index">
                <img :src="img.src" alt="">
                <p>{{img.text}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterTopComponent',
    data() {
        return {
            images: [
                {
                    src:  require("../assets/image/buy-comics-digital-comics.png"),
                    text: "digital comics",
                },
                {
                    src: require("../assets/image/buy-comics-merchandise.png"),
                    text: "dc merchandise",
                },
                {
                    src: require("../assets/image/buy-comics-subscriptions.png"),
                    text: "subscription",
                },
                {
                    src: require("../assets/image/buy-comics-shop-locator.png"),
                    text: "comic shop locator",
                },
                {
                    src: require("../assets/image/buy-dc-power-visa.svg"),
                    text: "dc power visa",
                },
            ],
        }

    },

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
        padding: 0 30px;
    }

    .image-special-link {
        @include imageflex;
        width: 100%;
    }

    & img{
        width: 4.375rem;
        margin-right: 0.625rem;

    }

    & p {
        text-transform: uppercase;
    }
}

</style>