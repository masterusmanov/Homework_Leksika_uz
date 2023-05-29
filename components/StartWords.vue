<template>
    <div class="container mx-auto flex justify-center items-center p-10">
        <div class="w-[60%] h-[100px] pl-5 rounded-2xl">
            <div class="p-5 flex justify-center items-center">
                <h1 class="text-3xl text-center">{{titles}}</h1>
            </div>
        </div>
    </div>
  </template>
  
  <script setup>

    defineProps(['titles'])  
    
  </script>
  
  <style lang="scss" scoped></style>