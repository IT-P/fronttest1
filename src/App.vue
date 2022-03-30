<template>
  <v-app>
    <v-app-bar color="primary"></v-app-bar>
    <v-navigation-drawer color="grey-darken-1" permanent></v-navigation-drawer>
    <v-main>
      <v-content>
        <v-container fluid fill-height>
          <v-layout align-center justify-center>
            <router-view></router-view>
          </v-layout>
        </v-container>
      </v-content>
    </v-main>
  </v-app>
</template>

<script>
import { mapState } from "vuex";

export default {
  name: "App",

  components: {},
  computed: {
    ...mapState(["user"]),
  },
};
</script>
