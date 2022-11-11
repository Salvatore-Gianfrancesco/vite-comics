<script>
import MainMenu from './MainMenu.vue';
export default {
    name: "SiteMain",
    components: {
        MainMenu
    }
}
</script>

<template>
    <main>
        <!-- Content Here Section -->
        <section class="content_here">
            <div class="container h-100">
                <div class="text d-flex align-items-center h-100 fs-4">Content goes Here</div>
            </div>
        </section>

        <!-- Main Menu Section -->
        <MainMenu />
    </main>
</template>

<style lang="scss">

</style>