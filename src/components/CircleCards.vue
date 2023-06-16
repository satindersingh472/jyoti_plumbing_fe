<template>
  <div>
    <v-container class="grid" fluid>
      <v-row no gutters justify-sm="center" >
        <v-col class="grid" cols="12" sm="6" lg="4" v-for="(circle, index) in circles" :key="index">
          <v-sheet tile  elevation="5" height="175px" width="175px" class="grid light-blue lighten-4 rounded-circle ">
            <v-icon size='50'  :color="circle['color']" >{{ circle["icon"] }}</v-icon>
            <p style="align-self:start;"  class="text-subtitle-2" >{{ circle['title'] }}</p>
        </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      circles: [
        {
            color:'green',
          icon: "mdi-home",
          title: "Residential Plumbing",
        },
        {
            color:'yellow darken-4',
            icon:'mdi-office-building',
            title:'Commercial Plumbing'
        },{
            color:'blue',
            icon:'mdi-water-alert',
            title:'Emergency Services'
        }
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.grid {
  display: grid;
  place-items: center;
}
</style>
