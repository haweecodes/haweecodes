<template>
  <v-app>
    <v-app-bar
      app
      flat
      absolute
      color="white"
      class="pt-6"
    >
    <v-spacer></v-spacer>
      <v-btn depressed class="nav-links" x-large color="white" to="/">Me</v-btn>
      <v-btn depressed class="nav-links" x-large color="white" to="/work">Work</v-btn>
    <v-spacer></v-spacer>
    </v-app-bar>
    <v-content>
      <v-container grid-list-md grid-list-xs grid-list-lg>
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  transition: 'layout',
}
</script>

<style>
.nav-links span {
  font-family: Raleway, sans-serif;
  font-size: 2em !important;
}
</style>
