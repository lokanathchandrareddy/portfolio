<template>
  <section class="bg-white p-6 rounded-lg shadow-md mt-8">
    <h2 class="text-2xl font-semibold mb-4">Work Experience</h2>
    <ul>
      <li v-for="job in jobs" :key="job.id" class="mb-6 border-b pb-4 flex items-center">
        <img :src="job.icon" alt="Company Logo" class="w-10 h-10 mr-4" />
        <div>
          <h3 class="text-xl font-bold">{{ job.position }} - {{ job.company }}</h3>
          <p class="text-gray-700">{{ job.description }}</p>
          <small class="text-gray-500">{{ job.date }}</small>
        </div>
      </li>
    </ul>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

interface Job {
  id: number
  position: string
  company: string
  description: string
  date: string
  icon: string
}

export default defineComponent({
  data() {
    return {
      jobs: [
        {
          id: 1,
          position: 'Front-End Engineer',
          company: 'Context Labs',
          description: 'Developed user-centric scalable applications.',
          date: 'Dec 2018 - Present',
          icon: '/context_labs_bv_logo.jpeg'
        },
        {
          id: 2,
          position: 'Software Engineer Intern',
          company: 'Incluvie',
          description: 'Built React components.',
          date: 'Aug 2018 - Dec 2018',
          icon: '/incluvie_logo.jpeg'
        },
        {
          id: 3,
          position: 'Analyst Programmer',
          company: 'Syntel ( now AtoS)',
          description: 'Programmer ',
          date: 'Dec 2013 - Aug 2016',
          icon: 'syntel_logo.jpeg'
        }
      ] as Job[]
    }
  }
})
</script>
<style scoped>
.experience {
  padding: 20px;
}
</style>
