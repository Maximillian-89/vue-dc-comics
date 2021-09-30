<template>
    <header>
        <div class="container-grid small-container">
            <nav class="box column-12">
                <div class="logo">
                    <img src="../assets/media/dc-logo.png" alt="Logo DC">
                </div>
                <ul>
                    <li><a href="#">CHARACTERS</a></li>
                    <li><a href="#">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
    export default {
        name: "Header"
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