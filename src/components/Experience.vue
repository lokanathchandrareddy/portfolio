<template>
  <section class="experience">
    <h2>Work Experience</h2>
    <ul>
      <li v-for="job in jobs" :key="job.id">
        <h3>{{ job.position }}</h3>
        <h4>{{ job.company }}</h4>
        <p>{{ job.description }}</p>
        <small> {{ job.date }}</small>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          id: 1,
          position: 'Front End Engineer',
          company: 'Context Labs Inc',
          description: 'Developed user-centric, scalable applications',
          date: 'Dec 2018 - Present'
        },
        {
          id: 2,
          position: 'Software Engineer - Intern',
          company: 'Incluvie',
          description: 'Built a netflix for short films website using React stack, ',
          date: 'Aug 2018 - Dec 2018'
        },
        {
          id: 3,
          position: 'Analyst Programmer',
          company: 'Syntel ( now AtoS)',
          description: 'Programmer ',
          date: 'Dec 2013 - Aug 2016'
        }
      ]
    }
  }
}
</script>
<style scoped>
.experience {
  padding: 20px;
}
</style>
