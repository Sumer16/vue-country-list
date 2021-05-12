<template>
  <header class="sticky w-full top-0 bg-gray-200 body-font z-10 shadow-lg dark:bg-gray-800">
    <div class="container mx-auto flex flex-wrap p-4 flex-row justify-between items-center">
      <a class="flex title-font font-medium items-center text-gray-800 hover:text-gray-700 focus:text-gray-700 mb-1 md:mb-0 cursor-pointer" href="./">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-10 h-10 text-white p-2 bg-indigo-500 rounded-full transform hover:-translate-y-1 transition duration-300 ease-in-out dark:text-gray-900" viewBox="0 0 24 24">
          <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"></path>
        </svg>
        <span class="ml-3 text-xl uppercase transition duration-300 ease-in-out dark:text-gray-300 dark:hover:text-gray-400 dark:focus:text-gray-400">Country List</span>
      </a>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>