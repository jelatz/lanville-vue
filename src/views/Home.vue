<template>
  <Hero />
  <div class="max-full mx-auto">
    <!-- OUR POPULAR PROGRAMS SECTION-->
    <Section variant="default" padding="xl">
      <div class="container">
        <h1 class="text-center text-4xl font-bold mb-10">
          Our Popular Programs
        </h1>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-20">
          <Card
            v-for="program in popularPrograms"
            :key="program.id"
            :title="program.title"
            :imageUrl="program.imageUrl"
            :imageAlt="program.imageAlt"
            imageHeight="h-64"
            shadow="xl"
            class="min-h-110"
            :hover="true"
          >
            <p class="line-clamp-6">
              {{ program.description }}
            </p>

            <button
              class="block ml-auto px-3 py-2 mt-4 bg-[#541517] text-white rounded hover:bg-[#3e0f11] transition duration-300 cursor-pointer"
              @click="handleSeeMore(program.id)"
            >
              See more
            </button>
          </Card>
        </div>
      </div>
    </Section>

    <!-- FEATURED PROGRAMS -->
    <Section variant="secondary" padding="xl">
      <div
        class="container flex justify-between items-start gap-15 flex-col md:flex-row"
      >
        <img
          src="../assets/images/hero-2.png"
          alt="Sample Image"
          class="w-140"
        />

        <p class="">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
          Necessitatibus ipsa at, adipisci quidem eligendi vitae vel atque
          explicabo cumque, reprehenderit doloribus voluptates itaque animi
          aperiam quisquam ab inventore delectus? Ab. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Ipsam nemo consequatur assumenda ut qui,
          aut cumque molestiae incidunt, dignissimos reiciendis fugiat
          consequuntur delectus, reprehenderit est inventore? Et animi nostrum
          praesentium! Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Nisi, minima cum ipsam voluptas quia deserunt consectetur, earum nobis
          praesentium, facere odit ullam. Fugit, possimus magni! Aperiam nemo
          debitis ratione aliquid.
        </p>
      </div>
    </Section>

    <!-- HOW IT WORKS -->
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import Hero from "@/components/Hero.vue";
import Section from "@/components/Section.vue";
import Card from "@/components/Card.vue";

interface Program {
  id: number;
  title: string;
  imageUrl: string;
  imageAlt: string;
  description: string;
}

const popularPrograms = ref<Program[]>([
  {
    id: 1,
    title: "Beautiful Landscape",
    imageUrl: "../../src/assets/images/hero-2.png",
    imageAlt: "Landscape photo",
    description: "Explore the beauty of nature. Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur sunt, at, soluta fugiat sit veniam incidunt porro laborum, dolore repellendus corrupti saepe quaerat cupiditate iure dolorum accusamus dolorem iste sed. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Corporis repudiandae beatae ipsam. Porro fugiat ea illum necessitatibus odio sed? Omnis commodi suscipit, nostrum quisquam perspiciatis eos. Culpa expedita ipsam perferendis?"
  },
  {
    id: 2,
    title: "Beautiful Landscape",
    imageUrl: "../../src/assets/images/hero-2.png",
    imageAlt: "Landscape photo",
    description: "Explore the beauty of nature. Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur sunt, at, soluta fugiat sit veniam incidunt porro laborum, dolore repellendus corrupti saepe quaerat cupiditate iure dolorum accusamus dolorem iste sed. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Corporis repudiandae beatae ipsam. Porro fugiat ea illum necessitatibus odio sed? Omnis commodi suscipit, nostrum quisquam perspiciatis eos. Culpa expedita ipsam perferendis?"
  },
  {
    id: 3,
    title: "Beautiful Landscape",
    imageUrl: "../../src/assets/images/hero-2.png",
    imageAlt: "Landscape photo",
    description: "Explore the beauty of nature. Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur sunt, at, soluta fugiat sit veniam incidunt porro laborum, dolore repellendus corrupti saepe quaerat cupiditate iure dolorum accusamus dolorem iste sed. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Corporis repudiandae beatae ipsam. Porro fugiat ea illum necessitatibus odio sed? Omnis commodi suscipit, nostrum quisquam perspiciatis eos. Culpa expedita ipsam perferendis?"
  }
]);

const handleSeeMore = (programId: number) => {
  // Navigate to program detail or show modal
  console.log(`Viewing program ${programId}`);
  // Example: router.push(`/programs/${programId}`)
};
</script>

<style scoped>
.container {
  max-width: 80rem;
  margin: 0 auto;
}
</style>
