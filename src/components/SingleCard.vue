<template>
    <div class="single-card">
        <img :src="card.thumb" :alt="card.series">
        <div class="title-card">{{card.series}}</div>
    </div>
</template>

<script>
    export default {
        name: "SingleCard",
        props: ['card'],
    }
</script>

<style lang="scss" scoped>
    .single-card {
        width: calc(100% / 6);
    }
</style>