<script setup>
   import {data} from "./data/data"
</script>

<template>
    <div class="card">
  <div class="card-header">
    {{ data.title }}
  </div>
  <div class="card-body">
    <blockquote class="blockquote mb-0">
      <h5 class=""> {{ data.heading }}</h5>
      <!-- <p>You have {{ data.task[2] }} task for today</p> -->
      <p>You have {{ data.task.length }} task for today</p>

      <footer class="blockquote-footer mt-5">{{ data.date() }} </footer>
    </blockquote>
  </div>
</div>
</template>

<style scoped>
</style>
