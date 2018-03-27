<template>
  <div class="project">
    <h2>{{ name }}</h2>
  </div>
</template>

<script>
export default {
  name: 'Project',
  props: ['name']
}
</script>

<style scoped>
.project {
  border: 1px solid #2c3e50;
  padding: 20px;
  margin: 20px 0;
}

h2 {
  margin: 0;
}
</style>
