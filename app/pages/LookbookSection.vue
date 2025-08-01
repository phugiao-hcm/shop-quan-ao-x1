<template>
  <section class="py-16 bg-white">
    <div class="container mx-auto px-4 text-center">
      <h2 class="text-3xl font-bold mb-6">Lookbook Mới Nhất</h2>
      <p class="text-gray-600 mb-10">
        Khám phá phong cách thời trang mới đầy cảm hứng
      </p>
      <div class="grid md:grid-cols-3 gap-6">
        <img
          v-for="i in 3"
          :key="i"
          :src="`/images/look${i}.jpg`"
          class="rounded-xl w-full h-80 object-cover"
        />
      </div>
    </div>
  </section>
</template>
