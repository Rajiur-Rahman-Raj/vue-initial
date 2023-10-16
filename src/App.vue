<script setup>

  const title1 = "<strong>lorem ipsum dummy text one</strong>";
  const title2 = "lorem ipsum dummy <em>text one</em>";

</script>

<template>
  <section>
      <h1 v-html="title1"></h1>
      <h2 v-html="title2"></h2>
  </section>
</template>

<style scoped>

</style>