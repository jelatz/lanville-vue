<template>
    <Hero />
    <div class="max-full mx-auto">
        <!-- WHO WE ARE SECTION-->
        <Section variant="default" padding="xl">
            <div class="container">
                <h1 class="text-center text-4xl font-bold mb-3">About Us</h1>
                
                <p class="w-180 block mx-auto">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Necessitatibus ipsa at,
                    adipisci quidem
                    eligendi
                    vitae vel atque explicabo cumque, reprehenderit doloribus voluptates itaque animi aperiam quisquam ab
                    inventore delectus? Ab. Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam nemo consequatur
                    assumenda ut qui, aut cumque molestiae incidunt, dignissimos reiciendis fugiat consequuntur delectus,
                    reprehenderit est inventore? Et animi nostrum praesentium! Lorem ipsum dolor sit amet consectetur
                    adipisicing elit. Nisi, minima cum ipsam voluptas quia deserunt consectetur, earum nobis praesentium,
                    facere
                    odit ullam. Fugit, possimus magni! Aperiam nemo debitis ratione aliquid.</p>
                </div>
        </Section>

        <!-- -->
        <Section variant="primary" padding="xl">
            <div class="container flex justify-between items-start gap-3 flex-col md:flex-row">
                <img src="../assets/images/hero-2.png" alt="Sample Image" class="w-140">
                
                <p class="">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Necessitatibus ipsa at,
                    adipisci quidem
                    eligendi
                    vitae vel atque explicabo cumque, reprehenderit doloribus voluptates itaque animi aperiam quisquam ab
                    inventore delectus? Ab. Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam nemo consequatur
                    assumenda ut qui, aut cumque molestiae incidunt, dignissimos reiciendis fugiat consequuntur delectus,
                    reprehenderit est inventore? Et animi nostrum praesentium! Lorem ipsum dolor sit amet consectetur
                    adipisicing elit. Nisi, minima cum ipsam voluptas quia deserunt consectetur, earum nobis praesentium,
                    facere
                    odit ullam. Fugit, possimus magni! Aperiam nemo debitis ratione aliquid.</p>
                </div>
        </Section>
    </div>


</template>

<script setup lang="ts">
import Hero from "@/components/Hero.vue";
import Section from "@/components/Section.vue";
</script>

<style scoped>
.container{max-width: 80rem;margin: 0 auto;}
</style>