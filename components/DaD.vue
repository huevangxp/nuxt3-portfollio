<template>
    <div class="flex bg-[#eaf3f3] p-2 rounded-lg">
      <div class="mx-10">
        <h1 class="text-2xl font-bold text-black">Favorite Foods</h1>
        <draggable v-model="meals" tag="ul" group="meals" class="bg-[#32908a] px-[100px] p-3  py-10 rounded-md">
          <template #item="{ element: meal }">
            <div class="w-60 bg-white my-2 rounded-xl text-[#000000] p-5">{{ meal }}</div>
          </template>
        </draggable>
      </div>
  
      <div>
        <h1 class="text-2xl font-bold text-black">Terrible Foods</h1>
        <draggable v-model="yuckyMeals" tag="ul" group="meals" class="bg-[#32908a] px-[100px]  p-3 py-10 rounded-md">
          <template #item="{ element: meal }">
            <div class="w-60 bg-white my-2 rounded-xl text-[#000000] p-5">{{ meal }}</div>
          </template>
        </draggable>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  import draggable from 'vuedraggable';
  
  const meals = ref([]);
  const yuckyMeals = ref([
    'Bat wing soup',
    'Spicy Octopus',
    'Anything from Taco Bell',
  ]);
  </script>
  