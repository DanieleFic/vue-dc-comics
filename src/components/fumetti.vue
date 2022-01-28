<template>
<div class="boxfumetti">
        <img :src="img.thumb" :alt="thumb.titolo">
        <h3>{{fumetti.titolo}}</h3>
    </div>
</template>

<script>
export default {
    name: 'fumetti',
    props: {
        'img': Object,
        'testo': String
    }
}
</script>

<style>
    .boxfumetti{
        height: 100px;
        width: 100px;
    }
</style>