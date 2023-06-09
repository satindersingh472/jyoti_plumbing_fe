<template>
  <v-app>
    <nav-bar></nav-bar>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import NavBar from './components/navbars/NavBar.vue';
export default {
  components:{NavBar},
  name: "App",
  metaInfo:{
    title: 'Jyoti Plumbing Solutions',
    titleTemplate: '%s | Jyoti Plumbing Solutions',
    link:[
            {
                rel:'icon',
                type: 'image/png',
                href: require("@/assets/logo.png")
            },

        ]
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
*{
  font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
</style>
