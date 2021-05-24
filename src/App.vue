<template>
  <v-app>
    <AppBar/>
    <v-main>
      <v-container>
        <router-view/>
      </v-container>
    </v-main>    
  </v-app>
</template>

<script>
// @ is an alias to /src
import AppBar from '@/components/AppBar.vue'

export default {
  components: {
    AppBar
  }
}
</script>

<style lang="scss">
</style>
