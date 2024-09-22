<template>
  <div id="app">
    <Header />
    <Skills />
    <Experience />
    <Education />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Header from './components/Header.vue'
import Skills from './components/Skill.vue'
import Experience from './components/Experience.vue'
import Education from './components/Education.vue'

export default defineComponent({
  components: {
    Header,
    Skills,
    Experience,
    Education
  }
})
</script>

<style scoped>
#app {
  font-family: 'Arial', sans-serif;
  padding: 20px;
}
</style>
