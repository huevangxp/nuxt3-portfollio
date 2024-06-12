<template>
    <div>
      <header class=" ">
        <nav class="flex justify-between items-center w-[92%] mx-auto py-4">
          <div>
            <img class="w-16 cursor-pointer" src="~/assets/images/dd.png" alt="School Logo">
          </div>
          <div
            class="nav-links duration-500 md:static absolute bg-[#32908a] md:min-h-fit min-h-[60vh] left-0 top-[-100%] md:w-auto w-full flex items-center px-5">
            <ul class="flex md:flex-row flex-col md:items-center md:gap-[4vw] gap-8">
              <li>
                <a class="hover:text-gray-500" href="#">Dashboard</a>
              </li>
              <li>
                <a class="hover:text-gray-500" href="#">Courses</a>
              </li>
              <li>
                <a class="hover:text-gray-500" href="#">Students</a>
              </li>
              <li>
                <a class="hover:text-gray-500" href="#">Teachers</a>
              </li>
              <li>
                <a class="hover:text-gray-500" href="#">Settings</a>
              </li>
            </ul>
            
          </div>
          <div class="flex items-center gap-6">
            <button class="bg-[#ffffff] font-bold text-[#32908a] px-5 py-2 rounded-full  ">Sign in</button>
          </div>
        </nav>
      </header>
    </div>
  </template>
  
  <script setup lang="ts"></script>
  
  <style scoped>
  header {
    position: sticky;
    top: 0;
    z-index: 50;
  }
  .nav-links {
    transition: top 0.5s;
  }
  </style>
  