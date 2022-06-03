<template>
   <div class="special-link">
       <div class="container">
            <div class="image-special-link" v-for="(img, index) in images" :key="index">
                <img :src="`/image/${src}`" alt="">
                <p>{{img.text}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SecondMainComponent',
    data() {
        return {
            images: [
                {
                    src: '../assets/image/dc-logo.png',
                    text: "digital comics",
                },
                {
                    src: '',
                    text: "dc merchandise",
                },
                {
                    src: '',
                    text: "subscription",
                },
                {
                    src: '',
                    text: "comic shop locator",
                },
                {
                    src: '',
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
        height: 50px;
    }

    & p {
        text-transform: uppercase;
    }
}

</style>