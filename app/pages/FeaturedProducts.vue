<template>
  <section class="py-12 px-4 md:px-8">
    <h2 class="text-3xl md:text-4xl font-bold text-center mb-10">
      Bộ sưu tập nổi bật
    </h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div
        v-for="(item, index) in featuredItems"
        :key="index"
        class="relative group overflow-hidden rounded-xl shadow-lg"
      >
        <img
          :src="item.image"
          alt="Featured"
          class="w-full h-96 object-cover transform group-hover:scale-105 transition duration-500"
        />
        <div
          class="absolute inset-0 bg-black/40 group-hover:bg-black/60 transition duration-300 flex items-center justify-center flex-col text-white text-center p-6"
        >
          <h3 class="text-2xl font-semibold mb-3">{{ item.title }}</h3>
          <p class="text-sm mb-5">{{ item.description }}</p>
          <NuxtLink
            :to="item.link"
            class="bg-white text-black font-medium px-5 py-2 rounded-full hover:bg-pink-600 hover:text-white transition"
          >
            Khám phá
          </NuxtLink>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const featuredItems = [
  {
    title: "Áo Khoác Mới Nhất",
    description: "Thời thượng, ấm áp và phong cách.",
    image: "/images/featured/jacket.jpg",
    link: "/collections/jackets",
  },
  {
    title: "Đầm Nữ Tinh Tế",
    description: "Dành cho những dịp đặc biệt.",
    image: "/images/featured/dress.jpg",
    link: "/collections/dresses",
  },
  {
    title: "Đầm Nữ Tinh Tế",
    description: "Dành cho những dịp đặc biệt.",
    image: "/images/featured/dress.jpg",
    link: "/collections/dresses",
  },
  {
    title: "Đầm Nữ Tinh Tế",
    description: "Dành cho những dịp đặc biệt.",
    image: "/images/featured/dress.jpg",
    link: "/collections/dresses",
  },
];
</script>
