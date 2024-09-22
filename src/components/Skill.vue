<template>
  <section class="bg-gray-100 p-6 rounded-lg shadow-md mt-8">
    <h2 class="text-2xl font-semibold mb-4">Skills</h2>
    <ul class="flex flex-wrap">
      <li
        v-for="skill in skills"
        :key="skill"
        class="bg-gray-200 p-2 m-2 rounded text-gray-800 font-semibold"
      >
        {{ skill }}
      </li>
    </ul>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      skills: ['Vue.js', 'Nuxt.js', 'React', 'JavaScript', 'Node.js', 'TypeScript', 'TailwindCSS'] as string[]
    }
  }
})
</script>

<style scoped>
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
