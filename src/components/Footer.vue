<template>
    <footer>
        <div class="bgd-footer-top">
            <div class="container-grid-footer small-container bgd-dc">
                <div class="column-12 footer-top">
                    <div>
                        <ul class="first-ul">
                            <li><h2>DC COMICS</h2></li>
                            <li v-for="(link, index) in footerLinks.dcComics" :key="index">
                                <a :href="link.link">{{link.name}}</a>
                            </li>
                            <li><h2>SHOP</h2></li>
                            <li v-for="(link, index) in footerLinks.shop" :key="index">
                                <a :href="link.link">{{link.name}}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li><h2>DC</h2></li>
                            <li v-for="(link, index) in footerLinks.dc" :key="index">
                                <a :href="link.link">{{link.name}}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li><h2>SITES</h2></li>
                            <li v-for="(link, index) in footerLinks.sites" :key="index">
                                <a :href="link.link">{{link.name}}</a>
                            </li>
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
                        <ul>
                            <li v-for="(link, index) in footerLinks.socials" :key="index">
                                <a :href="link.link"><img :src="'../media/' + link.src" :alt="link.alt"></a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>

<script>
    export default {
        name: "Footer",

        data() {
        return {
            footerLinks: {
                dcComics: [
                    {
                        name: 'Characters',
                        link: '#' 
                    },
                    {
                        name: 'Comics',
                        link: '#' 
                    },
                    {
                        name: 'Movies',
                        link: '#' 
                    },
                    {
                        name: 'TV',
                        link: '#' 
                    },
                    {
                        name: 'Games',
                        link: '#' 
                    },
                    {
                        name: 'Videos',
                        link: '#' 
                    },
                    {
                        name: 'News',
                        link: '#' 
                    }
                ],
                shop: [
                    {
                        name: 'Shop DC',
                        link: '#' 
                    },
                    {
                        name: 'Shop DC Collectibles',
                        link: '#' 
                    }
                ],
                dc: [
                    {
                        name: 'Terms Of Use',
                        link: '#' 
                    },
                    {
                        name: 'Privacy policy (New)',
                        link: '#' 
                    },
                    {
                        name: 'Ad Choices',
                        link: '#' 
                    },
                    {
                        name: 'Advertising',
                        link: '#' 
                    },
                    {
                        name: 'Jobs',
                        link: '#' 
                    },
                    {
                        name: 'Subscriptions',
                        link: '#' 
                    },
                    {
                        name: 'Talent Workshops',
                        link: '#' 
                    },
                    {
                        name: 'CPSC Certificates',
                        link: '#' 
                    },
                    {
                        name: 'Ratings',
                        link: '#' 
                    },
                    {
                        name: 'Shop Help',
                        link: '#' 
                    },
                    {
                        name: 'Contact Us',
                        link: '#' 
                    },
                ],
                sites: [
                    {
                        name: 'DC',
                        link: '#' 
                    },
                    {
                        name: 'MAD Magazine',
                        link: '#' 
                    },
                    {
                        name: 'DC Kids',
                        link: '#' 
                    },
                    {
                        name: 'DC Universe',
                        link: '#' 
                    },
                    {
                        name: 'DC Power Visa',
                        link: '#' 
                    },
                ],
                socials: [
                    {
                        src: 'footer-facebook.png',
                        link: '#',
                        alt: 'Icona FaceBook'
                    },
                    {
                        src: 'footer-twitter.png',
                        link: '#',
                        alt: 'Icona Twitter'
                    },
                    {
                        src: 'footer-youtube.png',
                        link: '#',
                        alt: 'Icona YouTube'
                    },
                    {
                        src: 'footer-pinterest.png',
                        link: '#',
                        alt: 'Icona Pinterest'
                    },
                    {
                        src: 'footer-periscope.png',
                        link: '#',
                        alt: 'Icona Locazione Shop'
                    }
                ]
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

    .container-grid-footer {
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        column-gap: 1.5rem;
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
    
    .first-ul {
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

        ul {
            display: flex;

            a {
                margin-left: .9375rem;
            }
        }
    }
</style>