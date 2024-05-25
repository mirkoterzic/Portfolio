<template>
  <div class="project-card">
    <h2>{{ project.title }}</h2>
    <a :href="project.github" target="_blank">GitHub</a>
    <a :href="project.live" target="_blank">Live Preview</a>
  </div>
</template>

<script>
export default {
  name: "ProjectCard",
  props: {
    project: Object,
  },
};
</script>

<style scoped>
.project-card {
  border: 1px solid #ddd;
  padding: 20px;
  border-radius: 5px;
}

.project-card h2 {
  margin: 0 0 10px 0;
}

.project-card a {
  display: block;
  margin-top: 10px;
  color: #3498db;
  text-decoration: none;
}
</style>
