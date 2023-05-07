<script setup></script>

<template>
  <main class="container">
    <input
      placeholder="Search for City"
      type="text"
      class="w-full px-1 mt-3 py-2 bg-transparent border-b focus:border-weather-secondary rounded-sm focus:outline-none"
    />
  </main>
</template>

<script setup>
import axios from "axios";
const getCity = async () => {
  const result = await axios.get(`https://v2.jokeapi.dev/joke/Any`);
  console.log(result.data.setup);
};

getCity();
</script>
