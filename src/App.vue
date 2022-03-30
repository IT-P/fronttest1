<template>
  <v-app>
    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import {mapState} from 'vuex';

export default {
  name: 'App',

  components: {
  },
  computed: {
    ...mapState(['user'])
  }
}
</script>
