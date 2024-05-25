<template>
  <div id="app">
    <About />
    <Projects />
    <Contact />
  </div>
</template>

<script>
import { defineComponent } from "vue";
import About from "./components/About.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";

export default defineComponent({
  name: "App",
  components: {
    About,
    Projects,
    Contact,
  },
});
</script>

<style src="./assets/styles/main.scss"></style>
