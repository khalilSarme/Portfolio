<template>
  <section-view>
    <template v-slot:title>
      <h4 class="text-h4 mb-4">My Certificates</h4>
    </template>
    <template v-slot:card-group>
      <v-row class="">
        <v-col cols="12" sm="6" md="4" lg="0" v-for="cer in cers" :key="cer">
          <v-card flat border>
            <v-card-text style="line-height: 0">
              <img :src="`../src/assets/${cer.src}`" alt="" class="w-100">
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </section-view>
</template>

<script setup>
  import {
    ref
  } from 'vue'
  
  const cers = ref([{
    src: 'cer_01.jpg'
  }, {
    src: 'cer_02.jpg'
  }, {
    src: 'cer_03.jpg'
  }])
</script>