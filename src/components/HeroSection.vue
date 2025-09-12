<template>
  <v-container class="fill-height">
    <v-row
      class="justify-center align-center flex-column-reverse flex-md-row"
      >
      <v-col cols="12" md="6">
        <h2 class="text-h2 mb-8">Khalil Al-Sarmy</h2>
        <h3 class="text-h3 mb-8 font-weight-thin">Front end web apps developer, <br> Web Designer for 4 years</h3>
        <v-btn class="elevation-0 rounded-xl mb-4 text-none" color="primary" href="https://t.me/KHALIL_NET_ITE" target="_blank">
          Chat me at Telegram
          <v-icon end icon="mdi-send"></v-icon>
        </v-btn>
      </v-col>
      <v-col class="text-center" cols="12" md="6">
        <v-avatar :size="300" class="elevation-1 mx-auto my-8">
          <v-img src="https://randomuser.me/api/portraits/men/22.jpg"></v-img>
        </v-avatar>
      </v-col>
    </v-row>
  </v-container>
</template>