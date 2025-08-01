<template>
    <section class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-10">
                Danh Mục Nổi Bật
            </h2>
            <div class="grid gap-6 grid-cols-2 md:grid-cols-4">
                <div
                    v-for="item in categories"
                    :key="item.id"
                    class="relative group cursor-pointer overflow-hidden rounded-xl"
                >
                    <img
                        :src="item.image"
                        alt=""
                        class="w-full h-64 object-cover transition-transform group-hover:scale-105"
                    />
                    <div
                        class="absolute bottom-0 w-full bg-black bg-opacity-50 text-white text-center py-2 font-semibold"
                    >
                        {{ item.name }}
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const categories = [
    { id: 1, name: "Áo Thun", image: "/images/1.png" },
    { id: 2, name: "Quần Jeans", image: "/images/2.png" },
    { id: 3, name: "Váy Nữ", image: "/images/3.png" },
    { id: 4, name: "Phụ Kiện", image: "/images/4.png" },
];
</script>
