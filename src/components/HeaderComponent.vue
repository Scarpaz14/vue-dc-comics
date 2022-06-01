<template>
    <div class="container">
        <header class="header">
            <div class="header__logo">
                <img src="../assets/image/dc-logo.png" alt="logo">
            </div>
            <nav class="header__nav">
                <ul>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                </ul>
            </nav>
        </header>
    </div>
</template>

<script>
export default {
    name:'HeaderComponent',

}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';
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
            padding: 1.25rem;
            text-decoration: none;
            color:var(--secondary-color)
        }

         a:hover{
            color: var(--primary-color);
        }
    }

}
</style>