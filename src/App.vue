<script>
import SiteHeader from "./components/SiteHeader.vue"
import SiteMain from "./components/SiteMain.vue"
import SiteFooter from "./components/SiteFooter.vue"
export default {
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<template>
  <!-- Site Header -->
  <SiteHeader />

  <!-- Site Main -->
  <SiteMain />

  <!-- Site Footer -->
  <SiteFooter />

</template>

<style lang="scss">
@use "./assets/scss/variables.scss" as *;

.content_here {
  height: 120px;
  background-color: $dark;
  color: $light;

  .text::before {
    content: "-->";
    padding-right: 0.5rem;
  }

  .text::after {
    content: "<--";
    padding-left: 0.5rem;
  }
}
</style>
