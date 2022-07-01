<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <Card />
  <Button text="about page button" />
</template>

<script>
import Card from "@/components/About/Card.vue";
import Button from "@/components/Button.vue";
export default {
  name: "AboutView",
  components: { Card, Button },
};
</script>