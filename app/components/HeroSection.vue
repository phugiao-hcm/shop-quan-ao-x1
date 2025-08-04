<template>
    <section
        class="relative bg-[url('/images/slider.png')] bg-cover bg-center bg-no-repeat h-[85vh] flex items-center justify-center"
    >
        <!-- Overlay -->
        <div
            class="absolute inset-0 bg-gradient-to-b from-black/60 to-black/40 z-0"
        ></div>

        <!-- Content -->
        <div class="relative z-10 text-white text-center px-6 md:px-10">
            <h1
                class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-4 drop-shadow-lg"
            >
                🌟 Khám Phá BST Mới Nhất 🌟
            </h1>
            <p
                class="text-base sm:text-lg md:text-xl mb-6 text-gray-200 max-w-2xl mx-auto drop-shadow"
            >
                Phong cách hiện đại, trẻ trung và độc đáo – tôn vinh vẻ đẹp của
                bạn trong từng đường nét.
            </p>
            <NuxtLink
                to="/"
                class="inline-block bg-pink-500 hover:bg-pink-600 focus:ring-4 focus:ring-pink-300 text-white font-semibold py-3 px-8 rounded-full shadow-lg transition-all duration-300 ease-in-out"
            >
                🛍️ Mua Ngay
            </NuxtLink>
        </div>
    </section>
</template>
