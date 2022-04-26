<template>
  <div class="mt-10 text-3xl mx-auto max-w-6xl">
    <Header />
    <div>HOST</div>

    <div>Count: {{ count }}</div>

    <div @click="addOne">Add one</div>

    <div>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from "vue";

const Header = defineAsyncComponent(() => import("remote/Header"));

export default {
  components: {
    Header
  },
  computed: {
    count() {
      return this.$store.state.count;
    }
  },
  methods: {
    addOne() {
      this.$store.commit('addOne');
    }
  }
}
</script>