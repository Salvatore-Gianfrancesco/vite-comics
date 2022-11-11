<script>
export default {
    name: "MainMenu",
    data() {
        return {
            menu: [
                {
                    text: "digital comics",
                    image: "buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    image: "buy-comics-merchandise.png"
                },
                {
                    text: "subscription",
                    image: "buy-comics-subscriptions.png"
                },
                {
                    text: "comic shop locator",
                    image: "buy-comics-shop-locator.png"
                },
                {
                    text: "dc power visa",
                    image: "buy-dc-power-visa.svg"
                }
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section class="main_menu ">
        <div class="container d-flex justify-content-evenly">
            <a href="#" v-for="item in menu" class="d-flex align-items-center">
                <img :src="getImageUrl(item.image)" alt="">
                <div class="text-uppercase ps-3">{{ item.text }}</div>
            </a>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables.scss" as *;

.main_menu {
    background-color: $primary_color;

    a {
        color: $light;
        text-decoration: none;
        white-space: nowrap;

        &:hover {
            text-decoration: underline;
        }
    }

    img {
        height: 50%;
        max-width: 50%;
    }
}
</style>