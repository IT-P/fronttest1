<template>
  <v-app>
    <v-app-bar app color="primary" prominent>
      <v-app-bar-nav-icon
        variant="text"
        @click.stop="drawer = !drawer"
      ></v-app-bar-nav-icon>
      v-app-bar
    </v-app-bar>

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
    <v-navigation-drawer
      app
      color="secondary"
      v-model="drawer"
      bottom
      permanent
    >
      v-navigation-drawer
    </v-navigation-drawer>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},
  data: () => ({
    drawer: true,
  }),
};
</script>
