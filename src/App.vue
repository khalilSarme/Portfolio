<template>
  <v-app :theme="theme">
    <custom-app-bar></custom-app-bar>
    <router-view></router-view>
    <custom-footer></custom-footer>
  </v-app>
</template>

<script setup>
  //
  import {
    ref,
    inject
  } from 'vue'

  const theme = ref('dark')
  const em = inject('em')

  em.on('tg_theme', () => {
    theme.value = (theme.value == 'light' ? 'dark': 'light')
  })
</script>
