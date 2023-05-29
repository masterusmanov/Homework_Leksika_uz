<template>
    <div class="bg-green-50 pt-5">
        <main class="container min-h-screen mx-auto p-10">
            <div class="grid bg-white">
                <div class="grid justify-center bg-white p-10 items-center mt-10">
                    <div>
                        <h1 class="text-4xl font-bold">TABLE OF CONTENTS</h1>
                    </div>    
                </div>
                <Table/>
            </div>
        </main>
    </div>
</template>

<script setup>
    const {name} = useRoute();
    useHead({
        title: `${name} page of Leksika.uz`,
        meta: [
        {
            name: "description", content: `${name} page of Leksika.uz`
        },
        {
            name: "author", content: "Leksika.uz"
        }
        ]
    })
</script>

<style lang="scss" scoped>

</style>