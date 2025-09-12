<template>
  <v-app-bar flat border class="px-2">
    <template v-slot:prepend>
      <v-app-bar-nav-icon border></v-app-bar-nav-icon>
    </template>
    <v-app-bar-title>
      Khalil Al-Sarmy
    </v-app-bar-title>
    <template v-slot:append>
      <v-btn :icon="themeicon" @click="tg_theme" class="border"></v-btn>
    </template>
  </v-app-bar>
</template>
<script setup>
  import {
    inject
  } from 'vue'

  const em = inject('em')

  const themeicon = ref("mdi-white-balance-sunny")

  const tg_theme = () => {
    themeicon.value = (themeicon.value == 'mdi-white-balance-sunny' ? 'mdi-weather-night': 'mdi-white-balance-sunny')
    em.emit('tg_theme')
  }

</script>