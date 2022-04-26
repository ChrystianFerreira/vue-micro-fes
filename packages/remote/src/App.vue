<template>
  <div class="bg-emerald-50 wrapper mt-10 text-3xl mx-auto max-w-6xl">
    <Header />
    <div>Name: remote</div>
    <div>Framework: vue3</div>
    <div>Language: JavaScript</div>
    <div>CSS: Tailwind</div>
  </div>
</template>

<script>
import Header from "./Header.vue";

export default {
  components: {
    Header
  }
}
</script>

<style scoped>
.vue-remote-color {
  background-color: #00C851;
}

.wrapper {
  height: 100vh;
  width: 100vh;
  margin: 0;
}
</style>