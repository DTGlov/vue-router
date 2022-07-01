<template>
  <h1>OOPs Page not Found</h1>
  <button @click="goHome">Home Page</button>
</template>

<script>
export default {
  name: "NotFound",
  methods: {
    goHome() {
      //   this.$router.push("/");
      this.$router.push({ name: "home" });
    },
  },
};
</script>

<style>
</style>