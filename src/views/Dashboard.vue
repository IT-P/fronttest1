<template>
  <v-card max-width="700" class="mx-auto">
    <v-card-title>
      Dashboard
    </v-card-title>
    <v-card-subtitle>
      For user {{ user.data.name }}
    </v-card-subtitle>
    <v-card-text>
      Dashboard text
    </v-card-text>
  </v-card>
</template>

<script>
import { mapState } from "vuex";
export default {
  computed: {
    ...mapState(["user"]),
  },
};
</script>
<style></style>
