<template>
    <header class="w-full md:px-3">
        <div class="p-4 w-full mx-auto flex justify-between items-center flex-col space-y-5 md:flex-row md:space-y-0">
            <a href="/"><img :src="logoName1" alt="Logo" class="w-62"></a>
            <div>
                <ul class="flex gap-2">
                    <li>
                        <Icon icon="mdi:facebook" class="w-8 h-8 text-blue-900" />
                    </li>
                    <li>
                        <Icon icon="mdi:instagram" class="w-8 h-8 text-red-400" />
                    </li>
                    <li>
                        <Icon icon="mdi:twitter" class="w-8 h-8 text-blue-400" />
                    </li>
                </ul>
            </div>
        </div>

        <nav class="relative">
            <!-- Mobile hamburger button -->
            <button @click="isMenuOpen = !isMenuOpen"
                class="md:hidden flex flex-col justify-center items-center w-8 h-8 mx-auto mb-4"
                aria-label="Toggle menu">
                <span class="block w-6 h-0.5 bg-gray-600 mb-1 transition-transform"
                    :class="{ 'rotate-45 translate-y-2': isMenuOpen }"></span>
                <span class="block w-6 h-0.5 bg-gray-600 mb-1 transition-opacity"
                    :class="{ 'opacity-0': isMenuOpen }"></span>
                <span class="block w-6 h-0.5 bg-gray-600 transition-transform"
                    :class="{ '-rotate-45 -translate-y-2': isMenuOpen }"></span>
            </button>

            <!-- Desktop menu -->
            <ul class="hidden md:flex  gap-10 justify-center **:hover:bg-[#541517] *:hover:text-white  py-2">
                <li class="*:p-3 *:w-full *:text-center *:block"><a href="/">Home</a></li>
                <li class="*:p-3 *:w-full *:text-center *:block"><a href="/about">About Us</a></li>
                <li class="*:p-3 *:w-full *:text-center *:block"><a href="">Programs</a></li>
                <li class="*:p-3 *:w-full *:text-center *:block"><a href="">Blog</a></li>
                <li class="*:p-3 *:w-full *:text-center *:block"><a href="">Contact Us</a></li>
            </ul>

            <!-- Mobile menu -->
            <ul v-show="isMenuOpen"
                class="md:hidden flex flex-col space-y-4 bg-white border-t border-gray-200 p-4 absolute top-full left-0 right-0 z-50 shadow-lg">
                <li><a href="/" class="block p-3 text-center hover:bg-[#541517] hover:text-white transition-colors"
                        @click="isMenuOpen = false">Home</a></li>
                <li><a href="/about" class="block p-3 text-center hover:bg-[#541517] hover:text-white transition-colors"
                        @click="isMenuOpen = false">About Us</a></li>
                <li><a href="" class="block p-3 text-center hover:bg-[#541517] hover:text-white transition-colors"
                        @click="isMenuOpen = false">Programs</a></li>
                <li><a href="" class="block p-3 text-center hover:bg-[#541517] hover:text-white transition-colors"
                        @click="isMenuOpen = false">Blog</a></li>
                <li><a href="" class="block p-3 text-center hover:bg-[#541517] hover:text-white transition-colors"
                        @click="isMenuOpen = false">Contact Us</a></li>
            </ul>
        </nav>
    </header>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import logoName1 from '@/assets/images/logo-name1.png';
import { MapPinIcon } from '@heroicons/vue/24/solid'
import { Icon } from '@iconify/vue';

const isMenuOpen = ref(false);
const title: string = "Lanville Academy";
</script>