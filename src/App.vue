<template>
  <v-app>
    <v-main>
      <!-- <pre>{{ user }}</pre> -->
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import {mapState} from 'vuex';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },
  computed: {
    ...mapState(['user'])
  }
}
</script>
