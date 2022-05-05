<template>
    <div class="card">
            <img :src="detail.thumb" :alt="detail.type">
            <h2>{{detail.series}}</h2>
    </div>
</template>

<script>
export default {
    name: 'ProductCard',
    data(){
        return{

        }
    },
    props: {
        detail: Object 
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.card{
    display: inline-block;
    margin: 0px 30px 60px;
    img{
        // width: 160px;
        height: 170px;
        // margin: 0px 30px;
    }
         h2{
        // padding: 10px 0;
        color: $bgwhite;
        font-size: 10px;
        text-transform: uppercase;
    }
}
</style>