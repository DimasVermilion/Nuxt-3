<template>
    <ProductDetails :product="product"/>

</template>

<script setup>
import ProductDetails from '~/components/ProductDetails.vue'

const {id} = useRoute().params
const url = 'https://fakestoreapi.com/products/' + id
definePageMeta({
    layout:'products'
})

const { data:product } = await useFetch(url)
 

</script>

<style scoped>

</style>