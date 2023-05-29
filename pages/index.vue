<template>
    <div class="bg-green-50 pt-10">
        <main class="min-h-screen">
            <div class="mt-10">
                <BtnSearch title="ENG ⇆ UZB" @search="handleSearch" />
                <div class="mt-10">
                    <StartWords titles="Search any words, and we found this word defination, translation and
                    etc."/>
                </div>
                <div class="mt-10">
                    <Search/>
                </div>
                <div class="mt-10">
                    <ErrorEng/>
                </div>
            </div>
        </main>
    </div>
  </template>
  
  <script setup>
    import BtnSearch from '../components/BtnSearch.vue'
    import { ref } from 'vue'

    const handleSearch = (value) => {
        console.log('Search value:', value)
    }

    const {name} = useRoute();
    useHead({
        title: `ENG ⇆ UZB page of Leksika.uz`,
        meta: [
        {
            name: "description", content: `ENG ⇆ UZB page of Leksika.uz`
        },
        {
            name: "author", content: "Leksika.uz"
        }
        ]
    })
  
  </script>
  
  <style lang="scss" scoped></style>