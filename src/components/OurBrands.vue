<template>
  <v-container class="mt-10">
    <v-row justify="center" no gutters>
      <v-col cols="12" style="display: grid; place-items: center">
        <p class="text-h4 indigo--text ">Our Trusted Brands</p>
        <p class="text-body-2" >We prefer top-most brands for the best results</p>
      </v-col>
    </v-row>
    <v-row justify="center">
      <v-col
        style="display: grid; place-items: center"
        cols="12"
        sm="6"
        md="4"
        lg="3"
        v-for="(brand, index) in brands"
        :key="index"
      >
        <v-img
          contain
          position="center"
          :src="require(`@/assets/brands/${brand['name']}.png`)"
          :alt="`Brand logo for ${brand['name']}`"
          width="200px"
          height="100px"
        ></v-img>
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
            name:'finolex'
        },
        {
            name:'astral'
        },
        {
            name:'ashirvad'
        },
        {
            name:'supreme'
        }
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
