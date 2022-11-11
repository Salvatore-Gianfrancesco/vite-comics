<script>
export default {
    name: "SiteHeader",
    data() {
        return {
            nav_items: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop",

            ]
        }
    }
}
</script>

<template>
    <header class="py-3">
        <div class="container d-flex justify-content-between">
            <!-- Logo -->
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </div>

            <!-- Navbar -->
            <nav class="navbar">
                <a href="#" v-for="item in nav_items" :class="(item === 'comics') ? 'active' : ''">
                    {{ item }}
                    <div class="active_bar"></div>
                </a>
            </nav>
        </div>
    </header>
</template>

<style lang="scss">
@use "../assets/scss/variables.scss" as *;

header {
    background-color: $light;

    img {
        height: 80px;
        aspect-ratio: 1/1;
    }

    a {
        color: $dark;
        text-decoration: none;
        text-transform: uppercase;
        margin: 1rem;
        position: relative;
        transition: 0.3s;

        &:hover {
            color: $primary_color;
        }

        .active_bar {
            height: 5px;
            width: 100%;
            position: absolute;
            bottom: -44px;
            left: 0;
        }

        &.active .active_bar {
            background-color: $primary_color;
        }

    }
}
</style>