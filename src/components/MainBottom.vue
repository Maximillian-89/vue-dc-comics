<template>
    <div class="bgd-main-bottom">
        <div class="container-grid small-container">
            <div class="main-bottom column-12">
                <ul>
                    <li><a href="#"><img src="../assets/media/buy-comics-digital-comics.png" alt="Icona Digital Comics"></a><span>DIGITAL COMICS</span></li>
                    <li><a href="#"><img src="../assets/media/buy-comics-merchandise.png" alt="Icona Merchandise"></a></li>
                    <li><a href="#"><img src="../assets/media/buy-comics-subscriptions.png" alt="Icona Sottoscrizione"></a></li>
                    <li><a href="#"><img src="../assets/media/buy-comics-shop-locator.png" alt="Icona Shop Locator"></a></li>
                    <li><a href="#"><img src="../assets/media/buy-dc-power-visa.svg" alt="Icona Visa"></a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "MainBottom"
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