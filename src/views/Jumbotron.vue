<template>
  <section class="dark:bg-gray-800  mt-14 dark:text-gray-100">
    <div class="container flex flex-col justify-center p-12 mx-auto sm:py-12 lg:py-24 lg:flex-row lg:justify-between">
      <div class="flex flex-col justify-center p-6 text-center rounded-sm lg:max-w-md xl:max-w-lg lg:text-left">
        <h6 class="text-blue-700 font-bold">Hi there, I am </h6>
        <h1 class="text-4xl font-bold leadi sm:text-4xl mb-5">Norman Bii
        </h1>
        <h1 class="text-2xl font-bold leadi sm:text-3xl">
          <span class="dark:text-violet-600"> <span class="text-gray-500">Professional</span> Web Developer</span>
        </h1>
        <p class="mt-6 mb-8 text-lg sm:mb-12">Professional Web Developer
          <br class="hidden md:inline lg:hidden">turpis pulvinar, est scelerisque ligula sem
        </p>
        <div
          class="flex flex-col space-y-4 sm:items-center sm:justify-center sm:flex-row sm:space-y-0 sm:space-x-4 lg:justify-start">

          <a href="#"
            class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-white rounded-lg bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 dark:focus:ring-blue-900">
            Contact Me
            <svg class="w-3.5 h-3.5 ml-2 rtl:rotate-180" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none"
              viewBox="0 0 14 10">
              <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M1 5h12m0 0L9 1m4 4L9 9" />
            </svg>
          </a>
          <a href="#"
            class="inline-flex justify-center items-center py-3 px-5 sm:ml-4 text-base font-medium text-center text-gray-900 rounded-lg border border-gray-300 hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800">
            Learn more
          </a>
        </div>
      </div>
      <div class="flex items-center justify-center p-6 mt-8 lg:mt-0 h-72 sm:h-80 lg:h-96 xl:h-112 2xl:h-128">
        <img src="../assets/Norman.jpeg" alt="Norman" class="object-contain h-72 sm:h-80 lg:h-96 xl:h-112 2xl:h-128">
      </div>
    </div>
  </section>
</template>

<script setup>
import { FwbCard } from 'flowbite-vue'
</script>
