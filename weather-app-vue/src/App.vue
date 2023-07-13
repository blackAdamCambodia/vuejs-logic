<script setup>
const location = "Dhaka"
const weather='t'
</script>

<template>
    <section class="container mx-auto flex items-center flex-col">
        <h1 class="text-center text-2xl py-10">Logic</h1>
        <div class="w-1/3 bg-gray-200 p-10 flex items-center flex-col space-y-10">
            <h1 class="text-3xl">{{ location }}</h1>
            
              <h2 v-if="weather == 's'" class="text-2xl">Weather: Sunny</h2>
              <h2 v-else-if="weather == 'pc'" class="text-2xl">Weather: Partly Cloudy</h2>
              <h2 v-else-if="weather == 'r'" class="text-2xl">Weather:Rainy</h2>
              <h2 v-else class="text-2xl">Weather: Thunderstorm</h2>

            <img v-if="weather == 's'" src="https://creazilla-store.fra1.digitaloceanspaces.com/icons/7911203/weather-icon-md.png" alt="">   
            <img v-if="weather == 'pc'" src="https://creazilla-store.fra1.digitaloceanspaces.com/icons/7912718/weather-icon-md.png" alt="">
            <img v-else-if="weather == 'r'" src="https://creazilla-store.fra1.digitaloceanspaces.com/icons/7913380/weather-icon-md.png" alt=""> 
            <img v-if="weather == 't'" src="https://creazilla-store.fra1.digitaloceanspaces.com/icons/7912589/weather-icon-md.png" alt="">
          
        </div>
    </section>
</template>

<style scoped>

</style>
