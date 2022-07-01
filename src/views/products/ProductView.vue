<template>
  <div v-for="product in products" :key="product.id">
    <router-link :to="{ name: 'productDetail', params: { id: product.id } }">{{
      product.name
    }}</router-link>
  </div>
</template>

<script>
import { productData } from "@/dummyData";

export default {
  name: "ProductView",
  computed: {
    products() {
      return productData;
    },
  },
};
</script>

<style scoped>
div {
  padding: 8px;
  background-color: gainsboro;
  margin: 10px auto;
  width: 200px;
}
</style>