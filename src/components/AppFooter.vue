<template>
    <footer>
        <div class="footer-top">
            <ul>
                <li><h3>Dc comics</h3></li>
                <li v-for="(link,index) in comics" :key="index">{{link.testo}}</li>
                <li><h3>Shop</h3></li>
                <li v-for="(link,index) in shop" :key="index">{{link.testo}}</li>
            </ul>

            <ul>
                <li><h3>Dc</h3></li>
                <li v-for="(link,index) in dc" :key="index">{{link.testo}}</li>
            </ul>

            <ul>
                <li><h3>Sites</h3></li>
                <li v-for="(link,index) in sites" :key="index">{{link.testo}}</li>
            </ul>
            <img src="../assets/images/dc-logo-bg.png" alt="">
        </div>
        <div class="footer-down">
            <div class="btn">
                <a href="#">Sign-up now!</a>
            </div>
            <div class="icons">
                <h4>Follow us</h4>
                <ul>
                    <li v-for="(icon,index) in icons" :key="index">
                        <img :src="icon.img" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name:'AppFooter',
    data(){
        return{
            comics:[
                {
                    testo: 'Characters',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Comics',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Movies',
                    link: '',
                    active: false,
                },
                {
                    testo: 'TV',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Games',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Videos',
                    link: '',
                    active: false,
                },
                {
                    testo: 'News',
                    link: '',
                    active: false,
                }
            ],
            shop:[
                {
                    testo: 'Shop DC',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Shop DC Collectibles',
                    link: '',
                    active: false,
                },
            ],
            dc:[
                {
                    testo: 'Terms of Use',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Privacy Policy(New)',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Ad choices',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Advertising',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Jobs',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Subscriptions',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Talent Workshops',
                    link: '',
                    active: false,
                },
                {
                    testo: 'CPSC Certificates',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Ratings',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Shop Help',
                    link: '',
                    active: false,
                },
                {
                    testo: 'Contact Us',
                    link: '',
                    active: false,
                },
            ],
            sites:[
                {
                    testo: 'DC',
                    link: '',
                    active: false,
                },
                {
                    testo: 'MAD Magazine',
                    link: '',
                    active: false,
                },
                {
                    testo: 'DC Kids',
                    link: '',
                    active: false,
                },
                {
                    testo: 'DC Universe',
                    link: '',
                    active: false,
                },
                {
                    testo: 'DC Power Visa',
                    link: '',
                    active: false,
                },
            ],
            icons:[
                {
                    img: require("../assets/images/footer-facebook.png")
                },
                {
                    img: require("../assets/images/footer-twitter.png")
                },
                {
                    img: require("../assets/images/footer-youtube.png")
                },
                {
                    img: require("../assets/images/footer-pinterest.png")
                },
                {
                    img: require("../assets/images/footer-periscope.png")
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables';

.footer-top{
    background-image: url("../assets/images/footer-bg.jpg");
    background-size: cover;
    width:100%;
    height: 300px;
    display: flex;
    overflow: hidden;
    position: relative;

    ul{
        list-style-type: none;
        padding: 0px 20px;
    }
    h3{
        color: $bgwhite;
        padding: 5px 0px;
        text-transform: uppercase;
    }
    li{
        color: $grey;
        padding: 2px;
    }
    img{
        position:absolute;
        top:-50px;
        right:100px;
        height: 130%;
    }
}

.footer-down{
    background-color: $bgfooter;
    display:flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 20px;

    .btn{
        border: 2px solid $blue;
        width: 140px;
        height: 50px;
        line-height: 50px;
        text-align: center;
    }
    a{  
        text-decoration: none;
        text-transform: uppercase;
        color: $bgwhite;
    }
    .icons{
        display: flex;
        justify-content: end;
    }
    h4{
        display: flex;
        align-items: center;
        text-transform: uppercase;
        color: $blue;
    }
    li{
        display:inline-block;
        list-style: none;
        padding: 10px;
    }
    img{
        width:100%;
    }
}
</style>