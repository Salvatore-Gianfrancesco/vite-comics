<script>
export default {
    name: "FooterSocial"
}
</script>

<template>
    <section class="footer_social py-4">
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <div class="col">
                    <div class="sign_now text-uppercase">sign-up-now!</div>
                </div>

                <div class="col d-flex justify-content-end align-items-center">
                    <a href="#" class="text-uppercase pe-3">follow us</a>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables.scss" as *;

.footer_social {
    background-color: $bg_footer;
    color: $light;

    .sign_now {
        border: 2px solid $primary_color;
        padding: 0.5rem;
        display: inline-block;
    }

    a {
        color: $primary_color;
        font-weight: bold;
        text-decoration: none;
    }

    img {
        padding: 0 0.5rem;
    }
}
</style>