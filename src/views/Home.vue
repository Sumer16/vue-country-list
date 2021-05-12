<template>
  <div class="bg-white h-full overflow-y-auto py-5 px-1 my-8 mx-1 grid grid-col md:grid-cols-3 sm:grid-cols-1 gap-6 justify-items-center dark:bg-gray-900">
    <!-- <h1 class="text-gray-900 dark:text-gray-100">Dark mode is here!</h1>
    <p class="text-gray-600 dark:text-gray-400">Welcome to Country List</p> -->
    <div v-for="arr in allCountries" :key="arr.name">
      <h5 class="text-gray-900 dark:text-gray-100">{{ arr.name }}</h5>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import axios from 'axios'

export default {
  name: 'Home',
  data() {
    return {
      allCountries: []
    }
  },
  created() {
    axios.get(`https://restcountries.eu/rest/v2/all`)
    .then(res => {
      const countries = res.data;
      for (const key of countries) {
        this.allCountries.push(key);
        console.log(key);
      }
    })
    .catch(err => {
      console.log(err);
    })
  }
}
</script>
