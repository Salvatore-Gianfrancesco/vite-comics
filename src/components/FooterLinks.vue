<script>
export default {
    name: "FooterLinks",
    data() {
        return {
            dc_comics: [
                {
                    text: "Characters",
                    href: "#"
                },
                {
                    text: "Comics",
                    href: "#"
                },
                {
                    text: "Movies",
                    href: "#"
                },
                {
                    text: "TV",
                    href: "#"
                },
                {
                    text: "Games",
                    href: "#"
                },
                {
                    text: "Videos",
                    href: "#"
                },
                {
                    text: "News",
                    href: "#"
                }
            ],
            shop: [
                {
                    text: "Shop DC",
                    href: "#"
                },
                {
                    text: "Shop DC Collectibles",
                    href: "#"
                }
            ],
            dc: [
                {
                    text: "Terms Of Use",
                    href: "#"
                },
                {
                    text: "Privacy policy (New)",
                    href: "#"
                },
                {
                    text: "Add Choices",
                    href: "#"
                },
                {
                    text: "Advertising",
                    href: "#"
                },
                {
                    text: "Jobs",
                    href: "#"
                },
                {
                    text: "Subscriptions",
                    href: "#"
                },
                {
                    text: "Talent Workshops",
                    href: "#"
                },
                {
                    text: "CPSC Certificates",
                    href: "#"
                },
                {
                    text: "Ratings",
                    href: "#"
                },
                {
                    text: "Shop Help",
                    href: "#"
                },
                {
                    text: "Contact Us",
                    href: "#"
                },
            ],
            sites: [
                {
                    text: "DC",
                    href: "#"
                },
                {
                    text: "MAD Magazine",
                    href: "#"
                },
                {
                    text: "DC Kids",
                    href: "#"
                },
                {
                    text: "DC Universe",
                    href: "#"
                },
                {
                    text: "DC Power Visa",
                    href: "#"
                }
            ]
        }
    }
}
</script>

<template>
    <section class="footer_links py-4">
        <div class="container">
            <div class="row justify-content-between">
                <!-- Links -->
                <div class="col">
                    <div class="container-fluid">
                        <div class="row justify-content-start">
                            <div class="col">
                                <!-- DC COMICS -->
                                <h5 class="text-uppercase">dc comics</h5>
                                <ul class="p-0">
                                    <li v-for="link in dc_comics"><a :href="link.href">{{ link.text }}</a></li>
                                </ul>

                                <!-- SHOP -->
                                <h5 class="text-uppercase">shop</h5>
                                <ul class="p-0">
                                    <li v-for="link in shop"><a :href="link.href">{{ link.text }}</a></li>
                                </ul>
                            </div>

                            <div class="col">
                                <!-- DC -->
                                <h5 class="text-uppercase">dc</h5>
                                <ul class="p-0">
                                    <li v-for="link in dc"><a :href="link.href">{{ link.text }}</a></li>
                                </ul>
                            </div>

                            <div class="col">
                                <!-- SITES -->
                                <h5 class="text-uppercase">sites</h5>
                                <ul class="p-0">
                                    <li v-for="link in sites"><a :href="link.href">{{ link.text }}</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Logo -->
                <div class="col">
                    <div class="logo">
                        <img src="../assets/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables.scss" as *;

.footer_links {
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    h5 {
        color: $light;
    }

    a {
        color: $gray;
        text-decoration: none;
    }

    .logo img {
        object-fit: contain;
    }
}
</style>