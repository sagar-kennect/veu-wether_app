<template>
  <header class="sticky top-0 bg-weather-primary shadow-lg">
    <nav
      class="container flex flex-col sm:flex-row items-center gap-4 text-white py-6"
    >
      <RouterLink :to="{ name: 'home' }">
        <div class="flex items-center gap-3">
          <i class="fa-solid fa-sun text-2xl cursor-pointer"></i>
          <p>The Local Weather</p>
        </div>
      </RouterLink>
      <div class="flex gap-3 flex-1 justify-end">
        <i
          class="fa-solid fa-circle-info hover:text-weather-secondary duration-150 cursor-pointer"
        ></i>
        <i
          class="fa-solid fa-plus hover:text-weather-secondary duration-150 cursor-pointer"
        ></i>
        <p @click="clickTest">Sagar</p>
      </div>

      <BaseModel>
        <div class="bg-white rounded-lg shadow-lg p-6">
          <div class="flex items-center mb-4">
            <img
              src="https://newprofilepic2.photo-cdn.net//assets/images/article/profile.jpg"
              alt="Profile Picture"
              class="w-16 h-16 rounded-full mr-4"
            />
            <h2 class="text-2xl font-bold">Our Team</h2>
          </div>
          <p class="text-gray-700 mb-4">
            We are a group of passionate individuals who are dedicated to
            delivering high-quality products and services to our clients. With
            years of experience in the industry, we have honed our skills and
            are always eager to learn and explore new technologies.
          </p>
        </div>
      </BaseModel>
    </nav>
  </header>
</template>

<script setup>
import { RouterLink } from "vue-router";
import BaseModel from "./BaseModal.vue";

const clickTest = () => {
  console.log("hello");
};
</script>
