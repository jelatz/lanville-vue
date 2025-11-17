<template>
    <header class="">
        <div class="p-4 w-400 mx-auto flex justify-between items-center">
            <a href="/"><img :src="logoName1" alt="Logo" class="w-62"></a>
            <div>
                <ul class="flex gap-2">
                    <li>
                        <Icon icon="mdi:facebook" class="w-10 h-10 text-blue-900" />
                    </li>
                    <li>
                        <Icon icon="mdi:instagram" class="w-10 h-10 text-red-400" />
                    </li>
                    <li>
                        <Icon icon="mdi:twitter" class="w-10 h-10 text-blue-400" />
                    </li>
                </ul>
            </div>
        </div>

        <!-- <MapPinIcon class="w-6 h-6 text-blue-500" /> -->
        <nav class="flex justify-center items-center py-5">
            <ul class="flex space-x-20 *:hover:underline *:text-lg">
                <li><a href="/">Home</a></li>
                <li><a href="/about">About Us</a></li>
                <li><a href="">Programs</a></li>
                <li><a href="">Blog</a></li>
                <li><a href="">Contact Us</a></li>
            </ul>
        </nav>
    </header>
</template>

<script setup lang="ts">
import logoName1 from '@/assets/images/logo-name1.png';
import { MapPinIcon } from '@heroicons/vue/24/solid'
import { Icon } from '@iconify/vue';




const title: string = "Lanville Academy";
</script>
