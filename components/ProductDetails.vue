<template>
    <div class="card">
        <div class="grid  grid-cols-2 gap-10">
            <div class="p-7">
                <img :src="product.image"" alt="foto" class="mx-auto my-7">
            </div>
            <div class="p-7">
                <h2 class="text-4x1 my-7">{{ product.title }}</h2>
                <p class="text-1x my-7">Price -${{ Product.price }}</p>
                <p class="text-1x my-7">{{ Product.description }}</p>
                <p class="text-1x my-7">{{ Product.category }}</p>
                <p class="text-1x my-7">{{ Product.id }}</p>

            </div>

        </div>

    </div>
</template>

<script setup>
const { product } = defineProps(['product'])

</script>

<style scoped>

</style>