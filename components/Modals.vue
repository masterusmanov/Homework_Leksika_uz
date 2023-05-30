<template>
    <div @click="open" class="w-full h-[180vh] bg-black bg-opacity-20 top-0 right-0 pt-[15%] left-0 flex justify-center items-center px-8 fixed z-50">
        <div class="p-10 bg-white self-start max-w-screen-md max-h-screen-xl">
            <h1 class="text-2xl font-bold">Asqar Arslonov</h1>
            <p class="mt-5 text-justify">Having started his IT-education at the age of 12, Asqarjon has reached the level of full-stack developer just 2 years later. Taking several online courses (Technical Support Fundamentals, Computer Networking) was followed by successful completion of Front-End Development and Back-End Development courses at the Open Web Academy education center in Qarshi city. Being an eighth-grader, he is fully responsible for the technical support of Leksika.uz</p>
            <button @click="emitClose" class="text-white mt-8 box-decoration-clone bg-blue-700 py-2 px-6 rounded-[20px]">Close</button>
        </div>
    </div>
</template>

<script setup>
import { defineEmits } from 'vue';

const emit = defineEmits(['close']);

function emitClose() {
  emit('close');
}
</script>

<style lang="scss" scoped>
</style>