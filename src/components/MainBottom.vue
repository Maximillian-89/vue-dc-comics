<template>
    <div class="bgd-main-bottom">
        <div class="container-grid small-container">
            <div class="main-bottom column-12">
                <ul>
                    <li v-for="(object, index) in objects" :key="index">
                        <a :href="object.link"><img :src="'../media/' + object.src" :alt="object.alt"></a><span>{{object.name}}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "MainBottom",

        data() {
        return {
            objects: {
                digitalComics: {
                    name: 'DIGITAL COMICS',
                    src: 'buy-comics-digital-comics.png',
                    link: '#',
                    alt: 'Icona Digital Comics'
                },
                merchandise: {
                    name: 'DC MERCHANDISE',
                    src: 'buy-comics-merchandise.png',
                    link: '#',
                    alt: 'Icona DC Merchandise'
                },
                subscription: {
                    name: 'SUBSCRIPTION',
                    src: 'buy-comics-subscriptions.png',
                    link: '#',
                    alt: 'Icona Sottoscrizione'
                },
                shopLocator: {
                    name: 'COMIC SHOP LOCATOR',
                    src: 'buy-comics-shop-locator.png',
                    link: '#',
                    alt: 'Icona Comic Shop'
                },
                cardVisa: {
                    name: 'DC POWER VISA',
                    src: 'buy-dc-power-visa.svg',
                    link: '#',
                    alt: 'Icona Visa'
                },
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

    .bgd-main-bottom {
        background-color: $mainColor;
    }

    ul {
        display: flex;
        justify-content: space-evenly;
    }

    li {
        display: flex;
        align-items: center;
        padding: 3.5rem 0;

        a {
            img{
                height: 2.5rem;
                margin-right: .625rem;
            }
        }

        span {
            color: #fff;
            cursor: pointer;
        }
    }
</style>