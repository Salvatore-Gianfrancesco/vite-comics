<script>
export default {
    name: "FooterLinks",
    data() {
        return {
            dc_comics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shop: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            dc: [
                "Terms Of Use",
                "Privacy policy (New)",
                "Add Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us"
            ],
            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ]
        }
    }
}
</script>

<template>
    <section class="footer_links">
        <div class="container">
            <div class="row justify-content-between">
                <!-- Links -->
                <div class="col-6 py-4">
                    <div class="container-fluid">
                        <div class="row justify-content-start">
                            <div class="col">
                                <!-- DC COMICS -->
                                <h5 class="text-uppercase">dc comics</h5>
                                <ul class="p-0">
                                    <li v-for="link in dc_comics"><a href="#">{{ link }}</a></li>
                                </ul>

                                <!-- SHOP -->
                                <h5 class="text-uppercase">shop</h5>
                                <ul class="p-0">
                                    <li v-for="link in shop"><a href="#">{{ link }}</a></li>
                                </ul>
                            </div>

                            <div class="col">
                                <!-- DC -->
                                <h5 class="text-uppercase">dc</h5>
                                <ul class="p-0">
                                    <li v-for="link in dc"><a href="#">{{ link }}</a></li>
                                </ul>
                            </div>

                            <div class="col">
                                <!-- SITES -->
                                <h5 class="text-uppercase">sites</h5>
                                <ul class="p-0">
                                    <li v-for="link in sites"><a href="#">{{ link }}</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Logo -->
                <div class="col-6">
                    <div class="logo h-100"></div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
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

        &:hover {
            text-decoration: underline;
        }
    }

    .logo {
        background-image: url("../assets/img/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
    }
}
</style>