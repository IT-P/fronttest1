<template>
  <v-app>
    <v-navigation-drawer app color="secondary" expand-on-hover>
      v-navigation-drawer
    </v-navigation-drawer>
    <v-app-bar app color="primary"> v-app-bar </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>
      <v-footer app color="primary" bottom fixed padless width="100%">
        v-footerv-footerv-footerv-footerv-footerv-footerv-footerv-footerv-footer
      </v-footer>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},
};
</script>
