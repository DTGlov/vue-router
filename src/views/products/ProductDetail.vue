<template>
  <button @click="back">Go Back</button>
  <button @click="forward">Go Forward</button>
  <h1>{{ product[0].name }}</h1>
  <img :src="product[0].ImageUrl" alt="" />
  <h3>${{ product[0].price }}</h3>
</template>

<script>
import { productData } from "@/dummyData";
export default {
  props: ["id"],
  methods: {
    back() {
      this.$router.go(-1);
    },
    forward() {
      this.$router.go(1);
    },
  },
  computed: {
    product() {
      return productData.filter((product) => product.id === this.id);
    },
  },
};
</script>

<style>
button {
  margin-right: 10px;
}
</style>