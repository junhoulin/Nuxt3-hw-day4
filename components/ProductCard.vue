<template>
  <div class="product-card">
    <CardImage :imageSrc="imageSrc" :altText="altText"></CardImage>
    <CardTitle :title="title"></CardTitle>
    <CardPrice :price="price"></CardPrice>
    <CardButton :buttonText="buttonText"></CardButton>
  </div>
</template>

<script setup>
defineProps({
  imageSrc: String,
  altText: String,
  title: String,
  price: String,
  buttonText: String,
})
</script>

<style scoped>
.product-card {
  border: 1px solid #ddd;
  border-radius: 8px;
  max-width: 300px;
  overflow: hidden;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}
</style>
