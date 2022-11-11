<script>
export default {
    name: "MainJumbotron"
}
</script>

<template>
    <section class="jumbotron">
        <div class="container h-100 position-relative">
            <div class="current_series text-uppercase">current series</div>
        </div>
    </section>
</template>

<style lang="scss">
@use "../assets/scss/variables.scss" as *;

.jumbotron {
    height: 20rem;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;

    .current_series {
        background-color: $primary_color;
        color: $light;
        font-weight: 600;
        padding: 0.5rem 1rem;
        display: inline-block;
        position: absolute;
        bottom: -20px;
        left: 0;
    }
}
</style>