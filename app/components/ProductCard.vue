<template>
  <div class="bg-white rounded-lg shadow hover:shadow-lg transition p-4">
    <img
      :src="product.image"
      :alt="product.name"
      class="w-full h-48 object-cover rounded"
    />
    <h2 class="text-lg font-semibold mt-2">{{ product.name }}</h2>
    <p class="text-pink-500 font-bold">{{ product.price }}₫</p>
  </div>
</template>

<script setup>
defineProps({ product: Object });
</script>
