<template>
<footer class="footer-top">
    <div class="container">
        <div class="footer__nav">
            <div class="col-footer">
                <h3>DC COMICS</h3>
                <ul>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                </ul>
                <h3>DC COMICS</h3>
                <ul>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                </ul>
            </div>
            <div class="col-footer">
                <h3>DC COMICS</h3>
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
            </div>
            <div class="col-footer">
                <h3>DC COMICS</h3>
                <ul>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                    <li><a href="">link</a></li>
                </ul>
            </div>
        </div>
         <div class="footer-logo">
            <img class="logo" src="../assets/image/dc-logo-bg.png" alt="">
        </div>
    </div>
</footer>
</template>

<script>
export default {
    name: 'FooterTopComponent'

}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

.container{
    display: flex;
    justify-content: space-between;
}

.footer-top{
    display: flex;
    align-items: center;
    background-image:url(../assets/image/footer-bg.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;

    & h3{
        color:white
    }

    & .col-footer{
       padding: 30px;
    }

    & ul {
        list-style: none;
    }

    & a{
        text-decoration: none;
        color: #959585;
    }

    & li{
        padding: 0.3125rem;
    }
}

.footer__nav{
    display: flex;
    width:100%;
}

.logo{ 
    width: 100%;
   display: block;
   object-fit: cover;
}

</style>