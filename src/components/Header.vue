<template>
    <header>
        <div class="container-grid small-container">
            <nav class="box column-12">
                <div class="logo">
                    <img src="../assets/media/dc-logo.png" alt="Logo DC">
                </div>
                <ul>
                    <li v-for="(elm, index) in nav" :key="index">
                        <a :href="elm.link"></a>{{elm.name}}
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
    export default {
        name: "Header",

        data() {
        return {
            nav: {
                characters: {
                    name: 'CHARACTERS',
                    link: '#',
                    // active: false
                },
                comics: {
                    name: 'COMICS',
                    link: '#',
                    // active: true
                },
                movies: {
                    name: 'MOVIES',
                    link: '#',
                    // active: false
                },
                tv: {
                    name: 'TV',
                    link: '#',
                    // active: false
                },
                games: {
                    name: 'GAMES',
                    link: '#',
                    // active: false
                },
                collectibles: {
                    name: 'COLLECTIBLES',
                    link: '#',
                    // active: false
                },
                videos: {
                    name: 'VIDEOS',
                    link: '#',
                    // active: false
                },
                fans: {
                    name: 'FANS',
                    link: '#',
                    // active: false
                },
                news: {
                    name: 'NEWS',
                    link: '#',
                    // active: false
                },
                shop: {
                    name: 'SHOP',
                    link: '#',
                    // active: false
                }
            }
        }
        
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

    header {
        padding: 2rem 0;
    }

    nav {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .logo {
        img {
            height: 5rem;
        }
    }

    ul {
        display: flex;
    }

    li {
        margin: 0 1.25rem;
        font-weight: 600;
        text-align: center;
        border-bottom: .3125rem solid transparent;
        cursor: pointer;

        &:hover {
            border-bottom: .3125rem solid $mainColor;
            transition-duration: .3s;
        }

        a {
            color: #000;
            text-decoration: none;

            &:hover {
                color: #00a9d9;
            }
        }
    }
</style>