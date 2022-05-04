<template>
    <div class="container">
        <div class="content">
            <h1>Content Goes Here</h1>
        </div>

        <div class="image-container">
            <ul v-for="(image, index) in images" :key="index">
                <li><img :src="image.img" :alt="image.testo"></li>
                <li>{{image.testo}}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name:'AppGrid',
    data(){
        return{
            images: [
                {
                    testo:'digital comics',
                    img: require("../assets/images/buy-comics-digital-comics.png"),
                    link: '',
                    active: true,
                },
                {
                    testo:'dc merchandise',
                    img: require("../assets/images/buy-comics-merchandise.png"),
                    link: '',
                    active: false,
                },
                {
                    testo:'subscription',
                    img: require("../assets/images/buy-comics-subscriptions.png"),
                    link: '',
                    active: false,
                },
                {
                    testo:'comic shop locator',
                    img: require("../assets/images/buy-comics-shop-locator.png"),
                    link: '',
                    active: false,
                },
                {
                    testo:'dc power visa',
                    img: require("../assets/images/buy-dc-power-visa.svg"),
                    link: '',
                    active: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables';

.content{
    background-color: $bgblack;
    padding: 10px;

    h1{
    color: $bgwhite;
    }
}

.image-container{
    background-color: $bgazzurro;
    display:flex;
    justify-content: space-around;

    ul{
        list-style-type: none;
        padding: 20px;
        text-transform: uppercase;
        color: $bgwhite;
        align-items: center;
        display: flex;
    }
    li{
        padding: 10px;
    }
    img{
        width:30px;
        height:40px;
    }
}
</style>