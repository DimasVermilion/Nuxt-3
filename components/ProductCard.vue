<template>
    <div class="card text-center">
        <img :src="product.image" alt="foto product" class="foto">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
        <nuxt-link :to="`/products/${product.id}`">
        <p class="btn my-4">View detail</p>
        </nuxt-link>
    </div>
</template>

<script setup>
const { product } = defineProps(['product'])

</script>

<style scoped>
.foto {
    max-height: 120px;
    max-width: 70%;
    margin: 0 auto;
  }

</style>