<template>
    <ul class="df-navigation">
        <li>
            <NuxtLink to="/" class=""> Home</NuxtLink>
            <NuxtLink to="/products" class=""> Products</NuxtLink>
        </li>
    </ul>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.df-navigation{
    padding:20px 0 ;
    li{
        a{
            padding:10px 15px;
        }
    }
}
</style>