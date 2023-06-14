<template>
  <div>
    <v-app-bar app flat elevate-on-scroll>
      <v-img contain src="@/assets/logo.png" width="50px" height="50px" position="center start"></v-img>
      <v-spacer></v-spacer>
      <mobile-nav-bar></mobile-nav-bar>
    </v-app-bar> 
  </div>
</template>

<script>
import MobileNavBar from './MobileNavBar.vue';
export default {
  components: { MobileNavBar },};
</script>

<style lang="scss" scoped></style>
