<template>
  <header class="bg-gray-800 text-white py-8 text-center">
    <h1 class="text-4xl font-bold">Lokanath ChandraReddy</h1>
    <div class="mt-4 flex justify-center space-x-4">
      <p>lokanathchandrareddy@gmail.com</p>
      <a href="https://github.com/lokanathchandrareddy" target="_blank">
        <Github />
      </a>
      <a href="https://linkedin.com/in/lokanathchandrareddy" target="_blank">
        <Linkedin />
      </a>
    </div>
  </header>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
import { Github, Linkedin } from 'lucide-vue-next'

export default defineComponent({
  components: {
    Github,
    Linkedin
  }
})
</script>
<style scoped>
.header {
  text-align: center;
  padding: 20px;
  background-color: #f0f0f0;
}
</style>
