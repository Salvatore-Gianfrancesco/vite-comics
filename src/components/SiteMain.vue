<script>
import MainJumbotron from './MainJumbotron.vue'
import MainComics from './MainComics.vue'
import MainMenu from './MainMenu.vue'
export default {
    name: "SiteMain",
    components: {
        MainJumbotron,
        MainComics,
        MainMenu
    }
}
</script>

<template>
    <main>
        <!-- Main Jumbotron -->
        <MainJumbotron />

        <!-- Main Comics -->
        <MainComics />

        <!-- Main Menu -->
        <MainMenu />
    </main>
</template>

<style lang="scss">

</style>