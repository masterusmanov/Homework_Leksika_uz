<template>
    <div v-for="el in cardView" :key="el.id" :card="el" class="card container mx-auto  m-5 shadow flex justify-beetwen p-5 items-center rounded-[20px] bg-white">
        <div class="w-1/3">
            <img src="../public/kitob.png" alt="">
        </div>
        <div class="w-1/2 text-gray-500 ml-10">
            <div>
                <i :class="el.icon" class='text-xl'></i><span class="ml-2 text-xl">{{el.text}}</span>
                <i :class="el.icon1" class='ml-10 text-xl'></i><span class="ml-2 text-xl">{{el.text1}}</span>
            </div>
            <div class="mt-5">
                <h1 class="text-[34px] text-black font-bold">{{el.title}}</h1>
            </div>
            <div>
                <p class="mt-5 text-justify text-black text-xl">{{el.text2}}</p>
            </div>
            <div class="mt-5 flex justify-end items-center">
                <nuxt-link :to="`/articles/${el.id}`" class="px-5 p-3 bg-teal-700 rounded-[20px] text-white">Batafsil</nuxt-link>
            </div>
        </div>
    </div>
  </template>
  
  <script setup>
    import { cardView } from '../constants/cardview';
  </script>
  
  <style lang="scss" scoped></style>