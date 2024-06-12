<script setup lang="ts"></script>

<template>
  <div class="background">
    <Header/>
    <div  class="background w-[70%]  mx-auto">
      <slot />
    </div>
  </div>
</template>

<style>
.background{
  background-color: #32908a;
  color: white;
  
}
</style>
