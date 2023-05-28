<template>
    <div class="container mx-auto flex justify-center items-center p-10">
        <div class="w-[80%] h-[74px] relative rounded-full bg-white flex justify-beetwen items-center">
            <nuxt-link to="#" class="bg-teal-700 mx-1 p-5 px-14 rounded-full text-white text-xl ">{{title}}</nuxt-link>
            <nuxt-link to="#"><i class='bx bx-search-alt-2 relative p-6 text-3xl text-gray-500 text-center'></i></nuxt-link>
            <input type="text" placeholder="Search words here..." class="w-[74%] pl-5 relative text-xl h-[74px] rounded-full">
        </div>
    </div>
  </template>
  
  <script setup>
    defineProps(['title'])  
  </script>
  
  <style lang="scss" scoped></style>