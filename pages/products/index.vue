<template>
<div>

    <section class="py-5">
        <div class="container">
            <div class="row g-4">
                <div class="col-md-3" v-for="(p,index) in product" :key="index">
                    <nuxt-link :to="`/products/${p.id}`">
                        <productCard :product="p" />
                    </nuxt-link>
                </div>
            </div>
        </div>
    </section>
</div>
</template>

<script setup>
const {
    data: product
} = await useFetch("https://api.escuelajs.co/api/v1/products");
</script>

<style  scoped>

</style>
