<template>
    <div class="container">
        <header class="header">
            <div class="header__logo">
                <img src="../../assets/image/dc-logo.png" alt="logo">
            </div>
            <nav class="header__nav">
                <ul>
                    <li v-for="(link, index) in links" :key="index"><a :href="link.url">{{link.text}}</a></li>
                </ul>
            </nav>
        </header>
    </div>
</template>

<script>
export default {
    name:'HeaderComponent',
    data() {
        return {
            links: [
                {
                    text: "Charcters",
                    url: "#",
                    current: false,
                },
                {
                    text: "comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "games",
                    url: "#",
                    current: false,
                },
                {
                    text: "collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "news",
                    url: "#",
                    current: false,
                },
                {
                    text: "shop",
                    url: "#",
                    current: false,
                },
            ],
        }
    },

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/mixins.scss';
.header{
    padding: 1.25rem 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    &__nav{
        ul{
            @include linkinline
        }


    a{
        margin: 0 1.25rem;
        text-decoration: none;
        color:var(--secondary-color);
        text-transform: uppercase;

    &:hover{
        color: var(--primary-color);
            }

    }
    }

}
</style>