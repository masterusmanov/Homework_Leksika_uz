<template>
    <form @submit.prevent class="container mx-auto flex justify-center items-center p-5 md:p-10">
        <div class="w-full md:w-[80%] h-[56px] md:h-[74px] shadow-lg shadow-teal-600 relative rounded-full bg-white flex justify-between items-center">
            <nuxt-link to="#" class="bg-teal-700 mx-1 p-3 md:p-5 px-10 md:px-14 rounded-full text-white text-base md:text-xl">{{titleq}}</nuxt-link>
            <button type="submit" @click="$emit('search', searchInput)"><i class='bx bx-search-alt-2 relative p-4 md:p-6 text-2xl md:text-3xl text-gray-500 text-center'></i></button>
            <input type="text" placeholder="Search words here..." v-model="searchInput" class="w-full md:w-[74%] pl-3 md:pl-5 relative border border-none focus:border-none focus:outline-none text-base md:text-xl h-[56px] md:h-[74px] rounded-full">
        </div>
      </form>
  </template>
  
  <script setup>
    defineProps(['titleq'])  
    import { ref, defineEmits } from 'vue'
    const searchInput = ref('')

    defineEmits(['search'])
  </script>
  
  <style lang="scss" scoped></style>