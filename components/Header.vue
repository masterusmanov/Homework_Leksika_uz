<template>
    <header class="bg-teal-700 h-[100px] flex ">
        <div class="container mx-auto flex justify-center items-center">
            <div class="w-1/2">
                <img src="../public/Logo.svg" alt="">
            </div>
            <div class="w-1/2 text-white flex justify-end text-xl">
                <ul class="flex gap-14">
                    <li><NuxtLink to="/">ENG ⇆ UZB</NuxtLink></li>
                    <li><NuxtLink to="/rus">RUS ⇆ UZB</NuxtLink></li>
                    <li><NuxtLink to="/articles">Articles</NuxtLink></li>
                    <li><NuxtLink to="/grammar">Grammar</NuxtLink></li>
                    <li><NuxtLink to="/about">About us</NuxtLink></li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script setup>

</script>

<style lang="scss" scoped>
    .router-link-exact-active {
        background-color: white;
        color: black;
        font-weight: 800;
        padding: 10px;
        border-radius: 20px;
    }
</style>