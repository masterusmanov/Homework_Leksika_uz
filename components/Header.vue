<template>
    <header class="bg-teal-700 h-[100px] flex sticky top-0 z-50 shadow ">
        <div class="container mx-auto flex justify-between items-center px-4 md:px-4">
            <div class="w-1/4 md:w-1/2">
                <img src="../public/Logo.svg" alt="">
            </div>
            <div class="w-2/3 md:w-1/2 text-white flex justify-end text-base ">
                <ul class="flex gap-4 md:gap-2">
                    <li class="md:w-[120px] text-center"><NuxtLink to="/">ENG ⇆ UZB</NuxtLink></li>
                    <li class="md:w-[120px] text-center"><p>RUS ⇆ UZB</p></li>
                    <li class="md:w-[120px] text-center"><NuxtLink to="/articles">Articles</NuxtLink></li>
                    <li class="md:w-[120px] text-center"><NuxtLink to="/grammar">Grammar</NuxtLink></li>
                    <li class="md:w-[120px] text-center"><NuxtLink to="/about">About us</NuxtLink></li>
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