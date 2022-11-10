<script>
export default {
    name: "MainMenu",
    data() {
        return {
            menu: [
                {
                    text: "digital comics",
                    href: "#",
                    img: "buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    href: "#",
                    img: "buy-comics-merchandise.png"
                },
                {
                    text: "subscription",
                    href: "#",
                    img: "buy-comics-subscriptions.png"
                },
                {
                    text: "comic shop locator",
                    href: "#",
                    img: "buy-comics-shop-locator.png"
                },
                {
                    text: "dc power visa",
                    href: "#",
                    img: "buy-dc-power-visa.svg"
                }
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container d-flex justify-content-between p-5">
            <a :href="item.href" v-for="item in menu">
                <!-- <img :src="'../assets/img/' + item.img" alt=""> -->
                <div class="text-uppercase">{{ item.text }}</div>
            </a>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables.scss" as *;

section {
    background-color: $primary_color;

    a {
        color: $light;
        text-decoration: none;
        transition: 0.3s;

        &:hover {
            text-decoration: underline;
        }
    }
}
</style>