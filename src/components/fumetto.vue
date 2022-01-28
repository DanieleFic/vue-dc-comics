<template>
<div class="boxfumetti">
        <img class="immaggini" :src="img" >
        <p>{{series}}</p>
    </div>
</template>

<script>
export default {
    name: 'fumetto',
    props: {
        'img': String,
        'series': String
    }
}
</script>

<style scoped lang="scss">
    .boxfumetti{
        width: 200px;
        height: 200px;
        padding: 15px 20px;
        margin: 10px 0px;
        background-size: contain;

        img{
            width: 100%;
            height: 100%;
        }


    }
</style>