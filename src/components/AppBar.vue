<template>
  <v-app-bar
    absolute
    color="#43a047"
    dark
    app
  >
    <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon> -->

    <v-toolbar-title class="ml-12">UnbiasedPost</v-toolbar-title>

    <v-spacer></v-spacer>

    <v-btn icon>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>

    <template v-slot:extension>
      <v-tabs align-with-title>
        <v-tab to="/">Home</v-tab>
        <v-tab to="/about">About Us</v-tab>
        <v-tab to="/contact">Contact Us</v-tab>
      </v-tabs>
    </template>
  </v-app-bar>
</template>

<script>
  export default {
    data() {
      return {}
    },
  }
</script>
