<template>
  <div class="home">
    <h1>This is the homePage</h1>
    <Banner />
    <Button text="home button" />
  </div>
</template>

<script>
import Banner from "@/components/Home/Banner.vue";
import Button from "@/components/Button.vue";
export default {
  name: "HomeView",
  components: { Banner, Button },
};
</script>
