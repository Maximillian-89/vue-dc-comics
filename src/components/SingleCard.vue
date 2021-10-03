<template>
    <div class="single-card">
        <img :src="card.thumb" :alt="card.series">
        <h4 class="title-card">{{card.series}}</h4>
    </div>
</template>

<script>
    export default {
        name: "SingleCard",
        props: ['card'], //**? Diamo un nome al props, che farà da elemento.
    }
</script>

<style lang="scss" scoped>

    .single-card {
        width: calc(100% / 6);
        padding: 0 .600rem;

        img {
            width: 100%;
            object-fit: cover;
            height: 12rem;
            object-position: top;
        }

        .title-card {
            color: #fff;
            margin-top: .9375rem;
            margin-bottom: 3.75rem;
        }
    }

</style>