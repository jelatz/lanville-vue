<template>
  <div class="min-h-dvh mx-auto">
    <!-- HERO -->
    <Section variant="default" padding="xl" sectionId="hero">
      <Hero :imageSrc="HeroMain">
        <div>
          <div class="bg-accent w-24 h-2 mb-10"></div>
          <h1 class="text-5xl lg:text-6xl font-bold leading-tight mb-6">Unlock Your Potential <span
              class="text-accent lg:block font-bold mt-1">Learn Limitlessly</span>
          </h1>
          <p class="leading-relaxed max-w-lg text-black text-lg lg:text-xl mb-8">Unlock your
            ptoential
            with world-class online tutorials. Expert instructors, flexible
            schedules, and personalized learning paths designed for your success.</p>
          <div class="flex flex-col lg:flex-row gap-4 w-full">
            <button
              class="bg-primary px-6 py-2 rounded text-white hover:-translate-y-2 hover:bg-[#0f2b60] transition-all duration-500">Explore
              Courses
              <ArrowRight class="w-6 h-6 inline-block" />
            </button>
            <button
              class="bg-transparent ring-1 ring-primary px-6 py-2 rounded text-primary hover:bg-[#0f2b60] hover:text-white transition-all">Watch
              Demo</button>
          </div>
        </div>
      </Hero>
    </Section>

    <!-- CORE VALUES -->
    <Section variant="default" class="lg:p-32 p-20">
      <div class="max-w-384 mx-auto grid grid-cols-1 md:grid-cols-3 lg:gap-12 gap-20">
        <div class="text-center">
          <Shield class="w-12 h-12 mx-auto text-accent mb-4" />
          <h3 class="font-bold text-xl mb-2">Integrity</h3>
          <p class="text-gray-700">We deliver honest, transparent, and reliable education.</p>
        </div>
        <div class="text-center">
          <Heart class="w-12 h-12 mx-auto text-accent mb-4" />
          <h3 class="font-bold text-xl mb-2">Passion</h3>
          <p class="text-gray-700">We are committed to inspiring lifelong learners worldwide.</p>
        </div>
        <div class="text-center">
          <Globe class="w-12 h-12 mx-auto text-accent mb-4" />
          <h3 class="font-bold text-xl mb-2">Accessibility</h3>
          <p class="text-gray-700">Education should be available to anyone, anywhere, anytime.</p>
        </div>
      </div>
    </Section>

    <!-- SERVICES -->
    <Section variant="primary" padding="md">
      <div class="max-w-394 mx-auto">
        <h1 class="text-5xl font-bold">
          Our <span class="text-accent">Services</span>
        </h1>

        <h2 class="text-2xl font-semibold mt-5">
          Online Learning Support for
          <span class="text-white">Elementary</span> to
          <span class="text-white">College Students</span>
        </h2>

        <Card :cards="services" imageClass="w-fit"
          containerClass="grid grid-cols-1 lg:grid-cols-3 gap-8 mt-10 max-w-6xl mx-auto" cardClass="shadow-xl"
          descriptionClass="text-white p-4" />
      </div>
    </Section>


    <!-- Subjects -->
    <Section class="py-24">
      <div class="max-w-6xl mx-auto px-6">
        <h2 class="text-5xl md:text-4xl font-bold text-left mb-6">
          What Can You <span class="text-accent">Learn?
          </span> </h2>

        <p class="text-left text-gray-600 max-w-2xl mb-16 text-2xl">
          We support students from elementary to college across core academic domains.
        </p>

        <div class="grid gap-10 lg:grid-cols-3">
          <div class="rounded-2xl p-8 bg-white shadow-xl hover:-translate-y-2 transition">
            <div class="text-4xl mb-4">🧮</div>
            <h3 class="text-xl font-semibold mb-3">Math & Logic</h3>
            <p class="text-gray-600">
              Arithmetic, Algebra, Geometry, Trigonometry, Calculus, Statistics
            </p>
          </div>

          <div class="rounded-2xl p-8 bg-white shadow-xl hover:-translate-y-2 transition">
            <div class="text-4xl mb-4">🔬</div>
            <h3 class="text-xl font-semibold mb-3">Science</h3>
            <p class="text-gray-600">
              General Science, Biology, Chemistry, Physics
            </p>
          </div>

          <div class="rounded-2xl p-8 bg-white shadow-xl hover:-translate-y-2 transition">
            <div class="text-4xl mb-4">✍️</div>
            <h3 class="text-xl font-semibold mb-3">Language & Communication</h3>
            <p class="text-gray-600">
              English, Reading Comprehension, Writing, Grammar
            </p>
          </div>
        </div>

        <div class="mt-20">
          <div
            class="rounded-3xl bg-linear-to-r from-accent to-primary text-white px-10 py-14 flex flex-col md:flex-row items-center justify-between gap-8 shadow-2xl">
            <div class="max-w-xl">
              <h3 class="text-3xl font-bold mb-3">
                Don't see your subject listed?
              </h3>
              <p class="text-blue-100 text-lg">
                We support a wide range of subjects and levels.
                Reach out and we'll help you find the right tutor.
              </p>
            </div>

            <a href="#contact"
              class="inline-flex items-center justify-center rounded-full bg-white text-blue-900 font-semibold px-8 py-4 text-lg hover:bg-blue-100 transition">
              Ask About Your Subject
            </a>
          </div>
        </div>

      </div>
    </Section>



    <!-- STATS -->
    <!-- <Section variant="default" padding="xl">
      <Stats :stats="stats" />
    </Section> -->

    <!-- WHY CHOOSE LANVILLE -->
    <Section variant="primary" padding="xl">
      <div class="max-w-384 mx-auto">
        <div class="bg-accent w-24 h-2 mb-10"></div>
        <h1 class="text-5xl lg:text-6xl font-bold leading-tight mb-6">Why Choose <span
            class="text-accent">Lanville?</span></h1>
        <p class="leading-relaxed max-w-lg text-white text-lg lg:text-xl mb-8">We combine cutting-edge technology
          with expert instruction to create an unparalleled learning experience.
        </p>

        <Card :cards="cardsWithIcons" iconClass="w-16 h-16 bg-accent p-4 rounded-lg hover:bg-[#f4b147]"
          descriptionClass="text-white p-4" cardClass="shadow-xl p-10" />
      </div>
    </Section>

    <!-- CONTACT FORM -->
    <Section variant="default" padding="xl" sectionId="contact">
      <div class="max-w-3xl mx-auto px-6">
        <!-- Accent bar -->
        <div class="bg-accent w-24 h-2 mb-8 rounded-full"></div>

        <!-- Heading -->
        <h2 class="text-4xl lg:text-5xl font-bold leading-tight mb-4">
          Contact <span class="text-accent">Us!</span>
        </h2>

        <!-- Subtitle -->
        <p class="text-gray-600 mb-10 text-lg">
          We're here to help. Fill out the form below and we'll get back to you as soon as possible.
        </p>

        <!-- Form -->
        <form action="#" class="bg-white shadow-xl rounded-2xl p-8 md:p-12 grid gap-6">
          <!-- Name -->
          <div class="flex flex-col">
            <label for="name" class="mb-2 font-semibold text-gray-700">Name</label>
            <input type="text" id="name" name="name" placeholder="Your full name"
              class="border border-gray-300 rounded-lg p-3 focus:outline-none focus:ring-2 focus:ring-accent focus:border-accent transition" />
          </div>

          <!-- Email -->
          <div class="flex flex-col">
            <label for="email" class="mb-2 font-semibold text-gray-700">Email</label>
            <input type="email" id="email" name="email" placeholder="your@email.com"
              class="border border-gray-300 rounded-lg p-3 focus:outline-none focus:ring-2 focus:ring-accent focus:border-accent transition" />
          </div>

          <!-- Message -->
          <div class="flex flex-col">
            <label for="message" class="mb-2 font-semibold text-gray-700">Message</label>
            <textarea id="message" name="message" rows="6" placeholder="Write your message here..."
              class="border border-gray-300 rounded-lg p-3 focus:outline-none focus:ring-2 focus:ring-accent focus:border-accent transition resize-none"></textarea>
          </div>

          <!-- Submit Button -->
          <button type="submit"
            class="bg-primary text-white font-semibold rounded-lg py-3 px-6 hover:bg-accent-dark transition shadow-md flex items-center justify-center gap-2">
            Send Message
          </button>
        </form>
      </div>
    </Section>

  </div>
</template>

<script setup lang="ts">
import Hero from "@/components/Hero.vue";
import Section from "@/components/Section.vue";
import "swiper/css";
import "swiper/css/pagination";
// import Stats from "@/components/Stats.vue";
import Card from "@/components/Card.vue";
// Icons
import { BookOpen, Zap, Award, Users, Globe, ArrowRight, Shield, Heart } from "lucide-vue-next";

import HeroMain from '@/assets/images/hero-main.jpg';

const services = [
  {
    id: 1,
    title: "Online Tutorial",
    imageUrl: HeroMain,
    description: "Personalized online tutorials designed to help students master core subjects at their own pace.",
  },
  {
    id: 2,
    title: "Test Preparation",
    imageUrl: HeroMain,
    description: "Focused exam reviews and practice sessions to help students perform confidently in tests.",
  },
  {
    id: 3,
    title: "Homework Assistance",
    imageUrl: HeroMain,
    description: "Guided homework support that helps students understand concepts, not just finish tasks.",
  },
]

// Cards (Why Choose Lanville Section)
const cardsWithIcons = [
  {
    id: 1,
    title: "Expert Instructors",
    icon: BookOpen,
    description: "Learn from industry professionals"
  },
  {
    id: 2,
    title: "Flexible Learning",
    icon: Zap,
    description: "Access thousands of courses"
  },
  {
    id: 3,
    title: "Community",
    icon: Award,
    description: "Join a vibrant learning community"
  },
  {
    id: 4,
    title: "Community Support",
    icon: Users,
    description: "Connect with fellow learners, get help from instructors, and collaborate on real-world projects"
  },
  {
    id: 5,
    title: "Global Access",
    icon: Globe,
    description: "Access quality education from anywhere in the world with our mobile-friendly platform and offline mode."
  },
  {
    id: 6,
    title: "Career Support",
    icon: Zap,
    description: "Get personalized career guidancem, job placement assistance, and industry connections to advance your career."
  }
];


</script>

<style scoped>
.container {
  max-width: 80rem;
  margin: 0 auto;
}
</style>
