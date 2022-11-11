<script>
import comics from "../data/comics.js"
import Comic from "./Comic.vue";
export default {
    name: "MainComics",
    components: {
        Comic
    },
    data() {
        return {
            comics
        }
    }
}
</script>

<template>
    <section class="main_comics pb-4">
        <div class="container">
            <div class="row row-cols-6 gx-3 py-5">
                <Comic class="col" v-for="comic in comics" :image="comic.thumb" :text="comic.series" />
            </div>
        </div>

        <div class="d-flex justify-content-center">
            <a href="#" class="text-uppercase">load more</a>
        </div>
    </section>
</template>

<style lang="scss">
@use "../assets/scss/variables.scss" as *;

.main_comics {
    background-color: $dark;
    color: $light;

    a {
        background-color: $primary_color;
        color: $light;
        font-weight: 600;
        text-decoration: none;
        padding: 0.5rem 4rem;

        &:hover {
            text-decoration: underline;
        }
    }
}
</style>