<template>
  <div>
    <h1>Projects</h1>

    <Project
      v-for="project of projects"
      :key="project.id"
      :name="project.name" />
  </div>
</template>

<script>
import Project from '@/components/Project'

export default {
  name: 'ProjectList',
  data () {
    return {
      projects: []
    }
  },
  components: {
    Project
  },
  created () {
    this.axios.get('/projects')
      .then(response => {
        this.projects = response.data.projects
      })
      .catch(e => {
        console.error(e)
      })
  }
}
</script>

<style scoped>

</style>
