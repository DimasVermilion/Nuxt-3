<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <ProductCard :product="p"/>

            </div>

        </div>
    </div>
</template>

<script setup>

const {id} = useRoute().params
definePageMeta({
    layout:'products'
})
 
const { data:products } = await useFetch('https://fakestoreapi.com/products')

</script>

<style scoped>

</style>