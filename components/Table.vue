<template>
    <div v-for="el in tables" :key="el.id" :acardion="el" class="accordion mt-10 flex justify-center items-center">
        <div class="accordion-item bg-teal-200 w-[80%]">
          <input type="checkbox" id="accordion-item-1" class="accordion-toggle" />
          <label for="accordion-item-1" class="accordion-title">
            <div class="flex justify-between items-center">
                <div class="w-1/2">
                    <b class="px-3 bg-teal-700 text-white p-1 rounded-full text-xl">{{el.id}}</b> <span class="font-bold text-2xl ml-5">{{el.title}}</span>
                </div>
                <div class="w-1/2 text-right">
                    <nuxt-link :to="`/grammar/${el.id}`"><b class="px-3 bg-white py-1 rounded-full text-xl">+</b></nuxt-link>
                </div>
            </div>
          </label>
          <!-- <div class="accordion-content bg-white">
              <nuxt-link to="#"><b class="px-3 bg-teal-700 text-white p-1 rounded-full text-xl ml-14">Batafsil</b></nuxt-link>
          </div> -->
        </div>
      </div>
    <div class="mt-10">
        
          
    </div>
</template>

<script setup>
    import {tables} from '../constants/table'
</script>

<style lang="scss" scoped>
    /* Accordion container */
.accordion {
    width: 100%;
  }
  
  /* Accordion item */
  .accordion-item {
    border-bottom: 1px solid #e2e8f0;
  }
  
  /* Accordion toggle */
  .accordion-toggle {
    display: none;
  }
  
  /* Accordion title */
  .accordion-title {
    display: block;
    padding: 1rem;
    cursor: pointer;
  }
  
  /* Accordion content */
  .accordion-content {
    padding: 1rem;
    display: none;
  }
  
  /* Toggle the content when the accordion item is checked */
  .accordion-toggle:checked ~ .accordion-content {
    display: block;
  }
</style>