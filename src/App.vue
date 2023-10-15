<script setup>
    const title = "Vue Js 3"
    const subtitle = "Start vue js 3 with project live";

    function getDate(){
      const date = new Date();
      return date.toDateString();
    }
</script>

<template>
    <div class="card">
  <div class="card-header">
    {{ title }}
  </div>
  <div class="card-body">
    <blockquote class="blockquote mb-0">
      <p> {{ subtitle }}</p>
      <footer class="blockquote-footer">{{ getDate() }} </footer>
    </blockquote>
  </div>
</div>
</template>

<style scoped>
</style>
