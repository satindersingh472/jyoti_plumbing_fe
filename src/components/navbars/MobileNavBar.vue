<template>
  <div>
    <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
    <v-navigation-drawer v-model="drawer" left clipped absolute height="100vh">
      <v-list>
        <v-list-item>
          <v-icon @click="drawer = false">mdi-close</v-icon>
        </v-list-item>
        <v-list-item-group v-model="group" class="text-body-1 text-center" v-for="(link,index) in links" :key="index" >
          <v-list-item>
            <v-list-item-title class="secondary--text" >{{ link['name'] }}</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      links: [
        {
          name: "Residential",
        },
        {
          name: "Commercial",
        },
        {
          name: "Emergency",
        },
        {
          name: "About Us",
        },
        {
          name: "Contact Us",
        },
        {
          name: "Location",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
