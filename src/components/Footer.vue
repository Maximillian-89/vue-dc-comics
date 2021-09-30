<template>
    <footer>
        <div class="bgd-footer-top">
            <div class="container-grid-footer small-container bgd-dc">
                <div class="column-12 footer-top">
                    <div>
                        <ul>
                            <li><h2>DC COMICS</h2> </li>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                            <li><h2>SHOP</h2></li>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li><h2>DC</h2></li>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li><h2>SITES</h2></li>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="bgd-footer-bottom">
            <div class="container-grid-footer small-container">
                <div class="column-12 box">
                    <div class="btn-sign">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="social">
                        <h2>FOLLOW US</h2>
                        <a href="#"><img src="../assets/media/footer-facebook.png" alt="Icona Facebook"></a>
                        <a href="#"><img src="../assets/media/footer-twitter.png" alt="Icona Twitter"></a>
                        <a href="#"><img src="../assets/media/footer-youtube.png" alt="Icona YouTube"></a>
                        <a href="#"><img src="../assets/media/footer-pinterest.png" alt="Icona Pinterest"></a>
                        <a href="#"><img src="../assets/media/footer-periscope.png" alt="Icona Localizzazione"></a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>

<script>
    export default {
        name: "Footer"
    }
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

    .container-grid-footer {
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        column-gap: 1.5rem;
        max-width: 100rem;
    }
    .bgd-footer-top {
        background-image: url("../assets/media/footer-bg.jpg");
        background-position: center top;
        background-repeat: no-repeat;
        background-size: cover;

    }
    .bgd-dc {
        background-image: url("../assets/media/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-position: right center;
        padding: 4rem 0rem;
    }

    .footer-top {
        display: flex;
    }

    .footer-top > div {
        margin-right: 3.75rem;
    }
    
    .footer-top > div > ul:first-child {
        li:nth-child(9) {
            margin-top: 16px;
        }
    }

    .footer-top > div > ul {
        li {
            h2 {
                color: #fff;
                margin-bottom: .625rem;
            }

            a {
                color: #959595;
                text-decoration: none;
                &:hover {
                    color: $mainColor;
                }
            }
        }
    }


    .bgd-footer-bottom {
        background-color: #303030;
        height: 6.75rem;
    }

    .btn-sign {
        button {
            background: #303030;
            border-color: $mainColor;
            border-style: solid;
            border-width: .125rem;
            color: #fff;
            font-size: 1.25rem;
            height: 3.125rem;
            margin-top: 1.875rem;
            padding: .4375rem;

            &:hover {
                background-color: $mainColor;
                text-decoration: none;
                cursor: pointer;
                transition-duration: .3s;
            }
        }
    }

    .box {
        justify-content: space-between;
    }

    .social {
        display: flex;
        margin-top: 1.875rem;
        align-items: center;

        h2 {
            color: $mainColor;
            margin-right: .9375rem;
        }

        a {
            margin-left: .9375rem;
        }
    }

</style>