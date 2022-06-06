<template>
        <div class="card">
            <img :src="thumb" :alt="title">
            <div class="title">
                <small>{{series}}</small>
            </div>
        </div>
</template>

<script>
export default {
    name: 'CardSeries',
    props: {
        thumb: String,
        series: String
    }
}
</script>

<style  lang="scss" scoped>
  img{
        height: 200px;
        width: 200px;
        object-fit: cover;
    }

    .title{
        color:white; 
        margin: 10px 0;
    }

    .card{
    width: 100%
}
</style>