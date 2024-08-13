<template>
    <div v-if="pending">
        <p>Loading...</p>
    </div>
    <div v-else class="grid grid-cols-5 gap-4">
        <div v-for="product in products" :key="product.id" class="flex flex-col shadow-md bg-white p-6 rounded-md">
            <img :src="product.image" alt="" class="h-auto self-center w-[75px]"/>
            <h3 class="text-black mt-auto text-sm">{{ product.title }}</h3>
        </div>
    </div>
</template>

<script setup>
const {
    pending, 
    data: products } = useFetch('https://fakestoreapi.com/products', {
    lazy:false,
    server: false
});

// const { data: products} = await useFetch('https://fakestoreapi.com/products');

</script>

<style lang="scss" scoped>

</style>