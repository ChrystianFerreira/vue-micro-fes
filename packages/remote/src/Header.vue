<template>
  <div>
    <div>
      <h1>Header component</h1>
      <p>@ Remote Vue App</p>
    </div>


    <div>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </div>

    <div>{{ count }}</div>
  </div>
</template>

<script>
export default {
  computed: {
    count() {
      return this.$store?.state?.count ?? 0;
    }
  }
}
</script>