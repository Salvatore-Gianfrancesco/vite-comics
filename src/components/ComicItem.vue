<script>
export default {
    name: "ComicItem",
    props: {
        image: String,
        text: String
    }
}
</script>

<template>
    <div>
        <img :src="image" :alt="text">
        <div class="text-uppercase pt-2 pb-4">{{ text }}</div>
    </div>
</template>

<style lang="scss">

</style>