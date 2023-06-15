<template>
  <v-app app>
    <nav-bar></nav-bar>
    <v-main >
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
