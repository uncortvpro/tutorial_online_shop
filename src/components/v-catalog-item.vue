<template>
  <div class="v-catalog-item">
    <img class="v-catalog-item__image" :src="require('../assets/images/'+product_data.image)" alt="">
    <p class="v-catalog-item__name">{{product_data.name}}</p>
    <p class="v-catalog-item__price">{{ product_data.price }} $</p>
    <button
        class="v-catalog-item__add_to_cart_btn btn"
        @click="sendDataToParent"
    >Add to cart</button>
  </div>
</template>

<script>
export default {
  name: "v-catalog-item",
  props: {
    product_data: {
      type: Object,
      default() {
        return {}
      }
    }
  },
  methods:{
    sendDataToParent(){
      this.$emit('sendArticle',this.product_data.article)
    }
  }
}
</script>

<style scoped>
.v-catalog-item__image{
  width: 100px;
}
.v-catalog-item {
  flex-basis: 25%;
  box-shadow: 0 0 8px 0 #e0e0e0;
  padding: 16px;
  margin-bottom: 16px;
}
</style>