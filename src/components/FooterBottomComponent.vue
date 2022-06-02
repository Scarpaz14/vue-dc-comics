<template>
<footer class="footer-bottom">
    <div class="container">
        <div class="btn-login">
            <button class="login">SIGN-UP-NOW!</button>
        </div>
        <div class="social-container">
            <div class="follow-us">
                <h4>FOLLOW US</h4>
            </div>
            <ul class="image-social">
                <li><a href=""><img src="../assets/image/footer-facebook.png" alt=""></a></li>
                <li><a href=""><img src="../assets/image/footer-twitter.png" alt=""></a></li>
                <li><a href=""><img src="../assets/image/footer-youtube.png" alt=""></a></li>
                <li><a href=""><img src="../assets/image/footer-pinterest.png" alt=""></a></li>
                <li><a href=""><img src="../assets/image/footer-periscope.png" alt=""></a></li>
            </ul>
        </div>
    </div>
</footer>
</template>

<script>
export default {
    name: 'FooterBottomComponent'

}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

.footer-bottom{
    background-color: #303030;
}

.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 6.25rem;

    & button{
        padding: 0.9375rem;
        border: 0.125rem solid #0282f9;
        background-color:inherit;
        color:white;
        font-weight: bold;
    }

    & .social-container{
        display: flex;
        align-items: center;

        & .image-social{
            display: flex;

            li{
                list-style: none;
            }
        }

        & img{
            margin: 0 0.625rem;
        }

        & h4{
            color: #0282f9;
            margin-right: 0.9375rem;
        }
    }
}



</style>