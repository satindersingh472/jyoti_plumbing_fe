<template>
  <div>
    <v-container class="grid mt-3">
      <v-row>
        <p class="primary--text text-h4"> <v-icon x-large class="primary--text" >mdi-map-marker-outline</v-icon> Locations</p>
      </v-row>
      <v-row no gutters>
        <v-col
          align-self="center"
          class="grid"
          cols="12"
          md="6"
          v-for="(location, index) in locations"
          :key="index"
        >
          <!-- <v-card-title class="font-weight-regular" >{{ location['name'] }}</v-card-title -->
          <v-card
            class="pa-4 grid grey lighten-2"
            shaped
            elevation="5"
            height="150px"
            width="300px"
          >
          <p>{{ location['street'] }}</p>
          <p>{{ location['city'] }}, {{ location['state'] }}</p>
            <!-- <v-card-text class="text-subtitle-2">
              {{ location["street"] }}, {{ location['city'] }}, {{ location['state'] }}
            </v-card-text> -->
            <v-card-actions
              ><v-btn class="secondary" :href="location['google_link']"
                >Get Directions</v-btn
              ></v-card-actions
            >
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      locations: [
        {
          name: "Devigarh",
          street: "Bhambuan Road (Opp. Shiv Mandir) ",
          city: "Devigarh",
          state: "Punjab",
          pincode: "147111",
          google_link: "https://goo.gl/maps/q17TPdftNxCNZELx5",
        },
        {
          name: "Naneola",
          street: "Near HDFC bank",
          city: "Naneola (Ambala) ",
          state: "Haryana",
          pincode: "144777",
        },
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
