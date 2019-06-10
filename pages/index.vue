<template>
  <section class="app-container">
    <top />
    <div class="background">
      <h1>Comida Oaxacana</h1>
      <!-- aka API -->
      <reviews />
    </div>
    <bottom />
  </section>
</template>

<!-- Added components for nav/footer and API -->
<script>
  import top from '~/components/top.vue'
  import bottom from '~/components/bottom.vue'
  import reviews from '~/components/reviews.vue'

  export default {
    components: {
      top,
      bottom,
      reviews
    }
  }
</script>

<style scoped>
.app-container {
  height: 100%;
  position: relative;
  display: grid;
  grid-template: auto 1fr auto / 1fr;
}

.background {
  background: url(~assets/lindsay-moe.jpg) center;
  background-size: cover;
  height: 100vh;
}
</style>
