<template>
  <v-app>
    <v-main>
      <slider/>
    </v-main>
  </v-app>
</template>

<script>
import slider from './components/slider';

export default {
  name: 'App',

  components: {
    slider,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
</style>
