<template>
  <transition name="fade">
    <div
      v-if="show"
      class="fixed inset-0 bg-black bg-opacity-60 z-50 flex items-center justify-center"
    >
      <div
        class="bg-white p-6 rounded-xl w-11/12 max-w-md text-center relative"
      >
        <button
          @click="show = false"
          class="absolute top-2 right-2 text-gray-500 hover:text-gray-800"
        >
          ✕
        </button>
        <h2 class="text-2xl font-bold mb-2 text-pink-600">Giảm giá 20%!</h2>
        <p class="mb-4 text-gray-700">
          Đăng ký nhận tin ngay để nhận mã giảm giá đặc biệt cho đơn hàng đầu
          tiên!
        </p>
        <input
          type="email"
          placeholder="Nhập email của bạn"
          class="w-full px-4 py-2 border rounded-lg mb-4"
        />
        <button
          class="bg-pink-500 text-white px-6 py-2 rounded-full hover:bg-pink-600"
        >
          Nhận mã
        </button>
      </div>
    </div>
  </transition>
</template>

<script setup>
import { ref, onMounted } from "vue";

const show = ref(false);

onMounted(() => {
  setTimeout(() => {
    show.value = true;
  }, 3000);
});
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease;
}
.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
