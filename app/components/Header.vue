<template>
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div
            class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center"
        >
            <!-- Logo -->
            <NuxtLink to="/" class="text-2xl font-bold text-gray-800">
                Fashion<span class="text-pink-500">Shop</span>
            </NuxtLink>

            <!-- Mobile menu button -->
            <button
                class="lg:hidden text-gray-800"
                @click="isOpen = !isOpen"
                aria-label="Toggle menu"
            >
                <svg
                    v-if="!isOpen"
                    class="w-6 h-6"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                >
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M4 6h16M4 12h16M4 18h16"
                    />
                </svg>
                <svg
                    v-else
                    class="w-6 h-6"
                    fill="none"
                    stroke="currentColor"
                    viewBox="0 0 24 24"
                >
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M6 18L18 6M6 6l12 12"
                    />
                </svg>
            </button>

            <!-- Navigation -->
            <nav
                :class="[
                    'flex flex-col lg:flex-row lg:items-center gap-4 lg:gap-6',
                    isOpen ? 'flex' : 'hidden lg:flex',
                    'absolute lg:static top-full left-0 w-full lg:w-auto bg-white lg:bg-transparent px-4 py-4 lg:p-0 shadow lg:shadow-none transition-all duration-300',
                ]"
            >
                <NuxtLink to="/" class="text-gray-800 hover:text-pink-500"
                    >Trang chủ</NuxtLink
                >
                <NuxtLink to="/" class="text-gray-800 hover:text-pink-500"
                    >Sản phẩm</NuxtLink
                >
                <NuxtLink to="/" class="text-gray-800 hover:text-pink-500"
                    >Giới thiệu</NuxtLink
                >
                <NuxtLink to="/" class="text-gray-800 hover:text-pink-500"
                    >Liên hệ</NuxtLink
                >
            </nav>
        </div>
    </header>
</template>

<script setup>
import { ref } from "vue";
const isOpen = ref(false);
</script>
