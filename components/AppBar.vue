<script>
import { mapActions } from 'vuex'
export default {
  methods: {
    ...mapActions(["toggleDialog"])
  }
}
</script>

<template>
  <v-app-bar
    flat
    color="transparent"
  >
    <div class="d-flex justify-space-between align-center">
      <img src="../assets/img/logo.png" style="width: 2.5em; height: 2.5em;" />
      <span class="ml-2 hidden-sm-and-down logo mt-n3">Oymo</span>
    </div>

    <v-spacer />

    <v-btn
      @click="toggleDialog"
      class="text-capitalize"
      depressed
      color="transparent"
    >
      About Us
    </v-btn>

    <v-btn
      @click="toggleDialog"
      class="text-capitalize"
      depressed
      color="transparent"
    >
      Services
    </v-btn>

    <v-btn
      @click="toggleDialog"
      class="text-capitalize hidden-xs-only"
      depressed
      color="transparent"
    >
      Parnership
    </v-btn>
  </v-app-bar>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Pacifico&display=swap");

.logo {
  font-family: "Pacifico", cursive !important;
  font-size: 2rem;
}
</style>