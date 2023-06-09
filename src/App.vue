<template>
  <v-app>
    <v-main>
      <indexView/>
    </v-main>
  </v-app>
</template>

<script>
import indexView from './components/IndexView.vue'

export default {
  name: 'App',

  components: {
    indexView,
  },

  data: () => ({
    //
  }),
}
</script>
