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
@import '../style/generals';

.card{
    margin: 0px 20px 60px;
    img{
        height: 150px;
        width: 150px;
    }
    h2{
        padding-top: 10px;
        color: $bgwhite;
        font-size: 12px;
        text-transform: uppercase;
        width: 160px;
    }
}
</style>