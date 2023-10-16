<script setup>

  const location = "dhaka"
  const weather = "rainy"


</script>

<template>
  <section>
      <h2>Location = {{ location }}</h2>
      <h2 v-if="weather == 'sunny'">Weather = Sunny</h2>
      <h2 v-else-if="weather == 'cloudy'">Weather = Cloudy</h2>
      <h2 v-else-if="weather == 'rainy'">Weather = Rainy</h2>
      <h2 v-else-if="weather == 'thundarstrom'">Weather = Thundarstrom</h2>
      <h2 v-else>No weather found</h2>

      <img v-if="weather == 'sunny'" src="./assets/images/sunny.png" alt="" width="200">
      <img v-else-if="weather == 'cloudy'" src="./assets/images/cloudy.png" alt="" width="200">
      <img v-else-if="weather == 'rainy'" src="./assets/images/rainy.png" alt="" width="200">
      <img v-else-if="weather == 'thundarstrom'" src="./assets/images/thunderstorm.png" alt="" width="200">
      <h4 v-else>No matching </h4>
  </section>
</template>

<style scoped>

</style>