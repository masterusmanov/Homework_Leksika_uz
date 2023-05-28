<template>
    <footer class="bg-teal-700 h-[70px] flex ">
        <div class="container mx-auto flex justify-center items-center">
            <div class="w-1/2">
                <h1 class="text-xl text-white">Leksika.uz - {{ new Date().getFullYear() }}</h1>
            </div>
            <div class="w-1/2 text-white flex gap-8 justify-end text-2xl">
                <nuxt-link to="#"><i class='bx bxl-telegram'></i></nuxt-link>
                <nuxt-link to="#"><i class='bx bxl-instagram' ></i></nuxt-link>
                <nuxt-link to="#"><i class='bx bxl-facebook' ></i></nuxt-link>
                <nuxt-link to="#"><i class='bx bxl-youtube' ></i></nuxt-link>
                <nuxt-link to="#"><i class='bx bxl-twitter' ></i></nuxt-link>
            </div>
        </div>
    </footer>
</template>

<script setup>

</script>

<style lang="scss" scoped>
</style>