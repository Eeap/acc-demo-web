<template>
  <v-app>
    <v-main style="background-color: black;">
      <Demo/>
    </v-main>
  </v-app>
</template>

<script>
import Demo from './components/Demo.vue'

export default {
  name: 'App',

  components: {
    Demo,
  },

  data: () => ({
    //
  }),
}
</script>
