<template>
  <v-app>
    <v-content>
      <Welcome/>
    </v-content>
  </v-app>
</template>

<script>
import Welcome from './components/Welcome';

export default {
  name: 'App',

  components: {
    Welcome,
  },

  data: () => ({
    //
  }),
};
</script>
