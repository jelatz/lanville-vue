<template>
    <footer class="bg-primary text-white pt-20">
        <div
            class="max-w-394 mx-auto px-6 grid grid-cols-1 lg:grid-cols-3 items-center place-items-center gap-12 mb-12">
            <!-- Logo & Tagline -->
            <div class="text-center lg:text-left w-full">
                <img :src="LogoWhite" alt="Lanville Academy Logo" class="h-20 w-auto mb-4">
                <p class="text-gray-200 text-md">
                    Empowering learners worldwide with quality education and career advancement opportunities.
                </p>
            </div>

            <!-- Bottom Bar -->
            <!-- <div class="py-8 max-w-6xl mx-auto px-6 flex flex-col md:flex-row items-center justify-between gap-6"> -->
            <p class="text-gray-300 text-right w-full">
                © {{ date }} Lanville Academy. All rights reserved.
            </p>

            <!-- Social Icons -->
            <div class="flex gap-4 justify-center lg:justify-end w-full">
                <a href="https://www.facebook.com/lanvilleacademy" class="hover:text-accent transition-colors">
                    <Facebook class="w-8 h-8" />
                </a>
                <a href="https://www.linkedin.com/lanvilleacademy" class="hover:text-accent transition-colors">
                    <Linkedin class="w-8 h-8" />
                </a>
                <a href="https://www.twitter.com/lanvilleacademy" class="hover:text-accent transition-colors">
                    <Twitter class="w-8 h-8" />
                </a>
            </div>
            <!-- </div> -->
        </div>
    </footer>
</template>

<script setup>
import { Facebook, Linkedin, Twitter } from 'lucide-vue-next';
import LogoWhite from '@/assets/images/logo-white.png'

const date = new Date().getFullYear();
</script>
