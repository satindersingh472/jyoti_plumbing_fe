<template>
  <v-app>
    <nav-bar></nav-bar>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>
import NavBar from '@/components/navbars/NavBar.vue'
export default {
  name: 'App',
components:{
  NavBar
},
  data: () => ({
    //
  }),
};
</script>
