<template>
  <section class="bg-gray-50 p-6 rounded-lg shadow-md mt-8">
    <h2 class="text-2xl font-semibold mb-4">Education</h2>
    <ul>
      <li v-for="edu in education" :key="edu.id" class="mb-6">
        <h3 class="text-xl font-bold">{{ edu.degree }}</h3>
        <p class="text-gray-700">{{ edu.institution }}</p>
        <small class="text-gray-500">{{ edu.date }}</small>
      </li>
    </ul>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

interface Education {
  id: number
  degree: string
  institution: string
  date: string
}

export default defineComponent({
  data() {
    return {
      education: [
        {
          id: 1,
          degree: 'Master of Science, Computer Science',
          institution: 'UMass Lowell',
          date: '2016 - 2018'
        },
        {
          id: 2,
          degree: 'Bachelor of Engineering, Information Science',
          institution: 'Visvesvaraya Technological University',
          date: '2009 - 2013'
        }
      ] as Education[]
    }
  }
})
</script>
