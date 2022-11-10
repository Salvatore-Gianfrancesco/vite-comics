<script>
import SiteHeader from "./components/SiteHeader.vue";
export default {
  components: {
    SiteHeader
  }
}
</script>

<template>
  <!-- Site Header -->
  <SiteHeader />

  <!-- Site Main -->
  <main>
    <section class="content_here">
      <div class="container h-100">
        <div class="text d-flex align-items-center h-100 fs-4">Content goes Here</div>
      </div>
    </section>
  </main>

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
