<script>
export default {
    name: "SiteHeader",
    data() {
        return {
            menu: [
                {
                    text: "characters",
                    href: "#"
                },
                {
                    text: "comics",
                    href: "#"
                },
                {
                    text: "movies",
                    href: "#"
                },
                {
                    text: "tv",
                    href: "#"
                },
                {
                    text: "games",
                    href: "#"
                },
                {
                    text: "collectibles",
                    href: "#"
                },
                {
                    text: "videos",
                    href: "#"
                },
                {
                    text: "fans",
                    href: "#"
                },
                {
                    text: "news",
                    href: "#"
                },
                {
                    text: "shop",
                    href: "#"
                },

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
                <a :href="item.href" v-for="item in menu" :class="(item.text === 'comics') ? 'active' : ''">
                    {{ item.text }}
                </a>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables.scss" as *;

header {
    background-color: $light;

    a {
        color: $dark;
        text-decoration: none;
        text-transform: uppercase;
        padding: 0 0.5rem;
        transition: 0.3s;

        &:hover {
            color: $primary_color;
        }

        &.active {
            color: $primary_color;
            text-decoration: underline;
        }
    }
}
</style>