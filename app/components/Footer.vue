<template>
    <footer class="bg-neutral-900 text-neutral-300 text-sm">
        <div
            class="max-w-7xl mx-auto px-4 py-10 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-8"
        >
            <!-- Cột 1: Phú Giáo Fashion -->
            <div>
                <h3 class="text-white font-semibold mb-4">Phú Giáo Fashion</h3>
                <ul class="space-y-2">
                    <li>
                        <NuxtLink to="/" class="hover:underline"
                            >Về chúng tôi</NuxtLink
                        >
                    </li>
                    <li>
                        <NuxtLink to="/" class="hover:underline"
                            >Tin tức</NuxtLink
                        >
                    </li>
                    <li>
                        <NuxtLink to="/" class="hover:underline"
                            >Cửa hàng</NuxtLink
                        >
                    </li>
                </ul>
            </div>

            <!-- Cột 2: Dịch vụ khách hàng -->
            <div>
                <h3 class="text-white font-semibold mb-4">
                    Dịch vụ khách hàng
                </h3>
                <ul class="space-y-2">
                    <li>
                        <NuxtLink to="/" class="hover:underline"
                            >Liên hệ</NuxtLink
                        >
                    </li>
                    <li>
                        <NuxtLink to="/" class="hover:underline"
                            >Chính sách đổi trả</NuxtLink
                        >
                    </li>
                    <li>
                        <NuxtLink to="/" class="hover:underline"
                            >Thanh toán & Giao hàng</NuxtLink
                        >
                    </li>
                </ul>
            </div>

            <!-- Cột 3: Kết nối -->
            <div>
                <h3 class="text-white font-semibold mb-4">
                    Kết nối với chúng tôi
                </h3>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:underline">Facebook</a></li>
                    <li><a href="#" class="hover:underline">Instagram</a></li>
                    <li><a href="#" class="hover:underline">YouTube</a></li>
                </ul>
            </div>

            <!-- Cột 4: Đăng ký nhận tin -->
            <div>
                <h3 class="text-white font-semibold mb-4">Đăng ký nhận tin</h3>
                <p class="mb-4">
                    Nhận thông tin khuyến mãi và bộ sưu tập mới nhất.
                </p>
            </div>
        </div>

        <div class="border-t border-neutral-700 text-center py-6 text-xs">
            © {{ new Date().getFullYear() }} Phú Giáo Fashion. All rights
            reserved.
        </div>
    </footer>
</template>
