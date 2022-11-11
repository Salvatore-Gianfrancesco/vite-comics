<script>
import MainJumbotron from './MainJumbotron.vue';
import MainMenu from './MainMenu.vue';
export default {
    name: "SiteMain",
    components: {
        MainJumbotron,
        MainMenu
    }
}
</script>

<template>
    <main>
        <!-- Main Jumbotron -->
        <MainJumbotron />

        <!-- Main Menu Section -->
        <MainMenu />
    </main>
</template>

<style lang="scss">

</style>