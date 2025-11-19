<script setup lang="ts">
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination, Autoplay } from "swiper/modules";
import "swiper/css";
import "swiper/css/pagination";
</script>

<template>
    <div class="w-full relative">
        <Swiper :slides-per-view="1" :autoplay="{ delay: 3000, disableOnInteraction: false }"
            :modules="[Navigation, Pagination, Autoplay]" :loop="true" :pagination="{ clickable: true }" class="h-130">
            <SwiperSlide>
                <img src="../assets/images/hero-1.webp" alt="image 1" class="w-full h-full object-cover" />
            </SwiperSlide>

            <SwiperSlide>
                <img src="../assets/images/hero-2.png" alt="image 2" class="w-full h-full object-cover" />
            </SwiperSlide>

            <SwiperSlide>
                <img src="../assets/images/hero-3.jpg" alt="image 3" class="w-full h-full object-cover" />
            </SwiperSlide>
        </Swiper>

        <div class="absolute inset-y-1/2 w-full md:inset-y-50 z-30">
            <div class="backdrop-blur-sm bg-black/30 rounded-r-xl border border-white/20 shadow-2xl p-8 max-w-3xl">
                <div class="text-center text-white">
                    <div class="text-xl md:text-2xl font-bold mb-4 drop-shadow-lg">Unlock Your Potential Through <span class="block">Quality Online Learning</span></div>
                    <p class="text-md md:text-md mb-6 drop-shadow-lg">Discover easy-to-follow tutorials and programs that empower you to grow, improve, and achieve your goals no matter where you are.</p>
                    <a href="#"
                        class="bg-[#541517] hover:bg-[#3e0f11] text-white font-semibold text-lg py-3 px-6 rounded-lg shadow-lg hover:shadow-xl transition duration-300 drop-shadow-lg">Explore
                        Programs</a>
                </div>
            </div>
        </div>
    </div>
</template>
