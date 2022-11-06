<template>
  <div class="v-catalog-item">
    <p>Item 1</p>
    <p>Price: 100</p>
    <p>Add to cart</p>
  </div>
</template>

<script>
export default {
  name: "v-catalog-item"
}
</script>

<style scoped>
  .v-catalog-item{
    flex-basis: 25%;
    box-shadow: 0 0 8px 0 #e0e0e0;
    padding: 16px;
    margin-bottom: 16px;
  }
</style>