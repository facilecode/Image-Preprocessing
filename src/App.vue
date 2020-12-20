<template>
  <v-app>

    <v-main>
      <Conv/>
    </v-main>
    
  </v-app>
</template>

<script>
import Conv from './components/Conv';

export default {
  name: 'App',

  components: {
    Conv,
  },

  data: () => ({
    //
  }),
};
</script>
