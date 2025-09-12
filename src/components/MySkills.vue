<template>
  <section-view>
    <template v-slot:title>
      <h4 class="text-h4 mb-4">My Skills</h4>
    </template>
    <template v-slot:card-group>
      <v-chip v-for="skill in skills" :key="skill" :color="skill.color" class="me-3 mt-3 border">
        <img :src="`../src/assets/${skill.src}`" alt="" width="20px" height="20px" class="me-2">
        {{ skill.text }}
      </v-chip>
    </template>
  </section-view>
</template>
<script setup>
  import {
    ref
  } from 'vue'

  const skills = ref([{
    src: 'html5logo.png',
    text: 'HTML 5',
    color: 'orange'
  }, {
    src: 'css3logo.png',
    text: 'CSS 3',
    color: 'light-blue'
  }, {
    src: 'jslogo.png',
    text: 'JavaScript',
    color: 'yellow-accent-4'
  }, {
    src: 'sass.png',
    text: 'SASS',
    color: 'pink-accent-2'
  }, {
    src: 'bootstrap.png',
    text: 'Bootstrap',
    color: 'deep-purple-accent-4'
  }, {
    src: 'jquery.png',
    text: 'JQuery',
    color: 'amber'
  }, {
    src: 'typescript.png',
    text: 'TypeScript',
    color: 'blue'
  }, {
    src: 'vuelogo.png',
    text: 'Vue js',
    color: 'teal'
  }, {
    src: 'logo.png',
    text: 'Vuetify js UI Framework',
    color: 'blue'
  }, {
    src: 'pinialogo.svg',
    text: 'Pinia',
    color: 'amber-accent-3'
  }, {
    src: 'vuelogo.png',
    text: 'Vuex',
    color: 'teal'
  }, {
    src: 'nodejs.png',
    text: 'Node js',
    color: 'green-accent-4'
  }, {
    src: 'expresslogo.png',
    text: 'Express js',
    color: 'blue-grey'
  }])
</script>