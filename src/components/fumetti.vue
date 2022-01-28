<template>
<div class="boxfumetti">
        <img :src="thumb.src" :alt="thumb.titolo">
        <h3>{{fumetti.titolo}}</h3>
    </div>
</template>

<script>
export default {
    name: 'fumetti',
    props: {
        'thumb': Object,
        'testo': String
    }
}
</script>

<style>

</style>