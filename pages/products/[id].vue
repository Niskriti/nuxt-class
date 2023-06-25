<template>
<div>
    <div class="container">
        <div class="row">
         <div class="col-md-4">
            <img :src="product.images[0]" alt="" class="img-fluid">
         </div>
         <div class="col-md-8">
            <div>
                <h1>{{ product.title }}</h1>
            </div>
            <div>
                <p>{{ product.description }}</p>
            </div>
            <div>
                <p>{{ product.price }}</p>
            </div>
            <div>
                <h6>category</h6>
                <p>{{ product.category.name }}</p>
                <img :src="product.category.image" alt="" width="80" class="rounded">
            </div>
            <div>
                <span><i class="fa-solid fa-circle-minus"></i></span>
                <span class="fs-1 px-5">1</span>
                <span><i class="fa-solid fa-circle-plus"></i></span>
            </div>
         </div>
        </div>
    </div>
</div>
</template>

<script setup>
     const route = useRoute();
     const {data:product} = await useFetch(`https://api.escuelajs.co/api/v1/products/${route.params.id}`)
</script>

<style scoped>

</style>
