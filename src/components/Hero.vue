<script setup lang="ts">
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination, Autoplay } from "swiper/modules";
import "swiper/css";
import "swiper/css/pagination";
</script>

<template>
    <Swiper :slides-per-view="1" :autoplay="{ delay: 3000, disableOnInteraction: false }"
        :modules="[Navigation, Pagination, Autoplay]" :loop="true" :pagination="{ clickable: true }" class="h-160">
        <SwiperSlide>
            <img src="../assets/images/logo-icon.png" alt="image 1" class="w-full h-full object-cover" />
        </SwiperSlide>

        <SwiperSlide>
            <img src="../assets/images/logo-name1.png" alt="image 2" class="w-full h-full object-cover" />
        </SwiperSlide>

        <SwiperSlide>
            <img src="../assets/images/logo-name2.png" alt="image 3" class="w-full h-full object-cover" />
        </SwiperSlide>
    </Swiper>
</template>
