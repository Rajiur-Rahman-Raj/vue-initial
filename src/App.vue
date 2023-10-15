<script setup>
    const title = "Vue Js 3"
    const subtitle = "Start vue js 3 with project live";

    const data = {
      title: "Vue Js 3",
      heading: "Start vue js course with Raju vai",
      date: () => {
        const date = new Date();
        return date.toDateString();
      },
      task:[1,2,3,4,5]
    }

    function getDate(){
      const date = new Date();
      return date.toDateString();
    }
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
