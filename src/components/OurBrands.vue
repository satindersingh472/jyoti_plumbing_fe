<template>
  <v-container class="mt-10">
    <v-row justify="center" no-gutters>
      <v-col align-self="center" cols="12" md="6">
        <p class="text-h4 text-md-h3 primary--text">Our Trusted Brands</p>
        <p class="primary--text font-weight-bold" >We care for customer's money</p>
        <p class="secondary--text">
          We prefer top-most brands for the best results. We give priority to
          the choice of a customer but still we do not compromise with the
          quality of the material. We work with top-of-the line brands and provide 100% free service guarantee for 10 years for our new customers.
        </p>
      </v-col>
      <v-col cols="12" md="6">
        <v-row justify="center">
          <v-col
            style="display: grid; place-items: center"
            md="6"
            v-for="(brand, index) in brands"
            :key="index"
          >
            <v-img
              contain
              position="center"
              :src="require(`@/assets/brands/${brand['name']}.png`)"
              :alt="`Brand logo for ${brand['name']}`"
              width="128px"
              height="100px"
            ></v-img>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      brands: [
        {
          name: "jaguar",
        },
        {
          name: "kohler",
        },
        {
          name: "cera",
        },
        {
          name: "hindware",
        },
        {
          name: "finolex",
        },
        {
          name: "astral",
        },
        {
          name: "ashirvad",
        },
        {
          name: "supreme",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/sass/variables.scss";
.regular-text {
  color: $regular-text;
}
</style>
