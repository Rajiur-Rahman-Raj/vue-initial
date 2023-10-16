<script setup>

  const location = "dhaka"
  const weather = "cloudy"


</script>

<template>
  <section>
      <h2>Location = {{ location }}</h2>

      <template v-if="weather == 'sunny'">
        <h2>Weather = Sunny</h2>
        <img src="./assets/images/sunny.png" alt="" width="200">
      </template>

      <template v-else-if="weather == 'cloudy'">
        <h2>Weather = Cloudy</h2>
        <img src="./assets/images/cloudy.png" alt="" width="200">
      </template>

      <template v-else-if="weather == 'rainy'">
        <h2>Weather = Rainy</h2>
        <img src="./assets/images/rainy.png" alt="" width="200">
      </template>

      <template v-else-if="weather == 'thundarstrom'">
        <h2>Weather = Thundarstrom</h2>
        <img src="./assets/images/thunderstorm.png" alt="" width="200">
      </template>

      <template v-else>
        <h2>Weather = No matching</h2>
      
      </template>
  </section>
</template>

<style scoped>

</style>