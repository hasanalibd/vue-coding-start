<script setup>
import {ref} from 'vue'

const number = ref(10)
const animal = ref('')
const searchUrl = 'https://www.pexels.com/search/'
</script>

<template>
  <div class="container mx-auto flex items-center justify-center min-h-screen flex-col">
      <h1 class="text-4xl">Welcome. Get ready to master Vue.js 3!</h1>
      <h2 class="mt-10 text-xl text-gray-700">{{ number }} / 4 = {{ number / 4 }}</h2>
      <h2 class="mt-10 text-xl text-gray-700">{{ number }} is {{ number % 2 == 0 ? "Even" : "Odd"  }}</h2>

      <input type="number" name="" id="" class="border-2 py-2 text-center" placeholder="Check Number" v-model="number">

      <!-- search option -->
      <!-- <h2 class="mt-10 text-xl text-gray-700">
        <a target="_blank" :href="searchUrl+animal.toLowerCase()">Search For {{ animal }}</a>
      </h2> -->
      
      <!-- dynamic search -->
      <h2 class="mt-10 text-xl text-gray-700">
        <a target="_blank" :href="`https://www.pexels.com/search/${animal.toLowerCase()}`">Search For {{ animal }}</a>
      </h2>

      <h2 class="mt-10 text-xl text-gray-700">
        <a target="_blank" :href="`https://www.pexels.com/search/${animal.toLowerCase()}`">Search For {{ animal }}</a>
      </h2>
      <input type="text" name="" id="" class="border-2 py-2 text-center" placeholder="search animals" v-model="animal">
  </div>
</template>

<style scoped>

</style>