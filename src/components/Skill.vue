<template>
  <section class="skills">
    <h2>Skills</h2>
    <ul>
      <li v-for="skill in skills" :key="skill">{{ skill }}</li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      skills: ['Vue.js', 'Nuxt.js', 'React', 'JavaScript', 'Node.js', 'TypeScript', 'TailwindCSS']
    }
  }
}
</script>
<style scoped>
.skills {
  padding: 20px;
}
.skills ul {
  list-style-type: none;
  display: flex;
  flex-wrap: wrap;
}
.skills li {
  margin-right: 15px;
  font-weight: bold;
}
</style>
