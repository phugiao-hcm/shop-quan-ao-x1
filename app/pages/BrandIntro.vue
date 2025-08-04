<template>
    <section class="py-20 bg-gray-900 text-white">
        <div
            class="container mx-auto px-4 grid md:grid-cols-2 items-center gap-8"
        >
            <div>
                <h2 class="text-4xl font-bold mb-4">
                    Thương Hiệu Của Chúng Tôi
                </h2>
                <p class="text-lg mb-6">
                    Chúng tôi mang đến những bộ sưu tập thời trang được thiết kế
                    tỉ mỉ và chất lượng cao, khơi gợi cá tính và phong cách
                    riêng biệt của bạn.
                </p>
                <NuxtLink
                    to="/"
                    class="inline-block bg-pink-500 hover:bg-pink-600 text-white font-semibold py-2 px-6 rounded-full transition"
                >
                    Xem thêm
                </NuxtLink>
            </div>
            <img
                src="/images/slider.png"
                alt="Brand"
                class="rounded-xl shadow-xl"
            />
        </div>
    </section>
</template>
