<template>
<footer class="footer-top">
    <div class="container">
        <div class="footer__nav">
            <div class="col-footer">
                <h3>DC COMICS</h3>
                <ul>
                    <li v-for="(link, index) in firstLinks" :key="index"><a :href="link.url">{{link.text}}</a></li>
                </ul>
                <h3>SHOP</h3>
                <ul>
                    <li v-for="(link, index) in secondLinks" :key="index"><a :href="link.url">{{link.text}}</a></li>
                </ul>
            </div>
            <div class="col-footer">
                <h3>DC</h3>
                <ul>
                    <li v-for="(link, index) in thirdLinks" :key="index"><a :href="link.url">{{link.text}}</a></li>
                </ul>
            </div>
            <div class="col-footer">
                <h3>SITES</h3>
                <ul>
                    <li v-for="(link, index) in fourthLinks" :key="index"><a :href="link.url">{{link.text}}</a></li>
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
    name: 'FooterMediumComponent',
     data() {
        return {
            firstLinks: [
                {
                    text: "Charcters",
                    url: "#",

                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Video",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",

                },
            ],

            secondLinks:[
                {
                    text: "Shop DC",
                    url: "#",
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                },

            ],

            thirdLinks: [
                {
                    text: "Term of use",
                    url: "#",
                },
                {
                    text: "Privacy Policy",
                    url: "#",
                },
                {
                    text: "Ad choice",
                    url: "#",

                },
                {
                    text: "Advertising",
                    url: "#",
                },
                {
                    text: "Jobs",
                    url: "#",
                },
                {
                    text: "Subscrition",
                    url: "#",
                },
                {
                    text: "Talent workshop",
                    url: "#",
                },
                {
                    text: "CPSC Certificates",
                    url: "#",
                },
                {
                    text: "Ratings",
                    url: "#",
                },
                {
                    text: "Shop help",
                    url: "#",
                },
                {
                    text: "Contact us",
                    url: "#",
                },
            ],
               fourthLinks: [
                {
                    text: "DC",
                    url: "#",
                },
                {
                    text: "MAD magazine",
                    url: "#",
                },
                {
                    text: "DC kids",
                    url: "#",
                },
                {
                    text: "DC universe",
                    url: "#",
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                },
            ],
        }
    },

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
        color:white;
        margin-bottom: 0.625rem;
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

    & a:hover{
        color:var(--primary-color);
    }

    & li, h3{
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