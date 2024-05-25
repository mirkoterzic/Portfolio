<template>
  <section class="projects">
    <h1>Projects</h1>
    <div class="project-list">
      <ProjectCard
        v-for="project in projects"
        :key="project.id"
        :project="project"
      />
    </div>
  </section>
</template>

<script>
import ProjectCard from "./ProjectCard.vue";

export default {
  name: "Projects",
  components: {
    ProjectCard,
  },
  data() {
    return {
      projects: [
        { id: 1, title: "Project One", github: "#", live: "#" },
        { id: 2, title: "Project Two", github: "#", live: "#" },
        { id: 3, title: "Project Three", github: "#", live: "#" },
        { id: 4, title: "Project Four", github: "#", live: "#" },
      ],
    };
  },
};
</script>

<style scoped>
.projects {
  padding: 20px;
}

.project-list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
</style>
