<template>
  <div>
    <v-container
      fluid
      class="fill-height"
      style="display: grid; place-items: center"
    >
      <v-row justify="center">
        <v-col
        order="2"
        cols="12"
        md="6"
          class="md-mt-2 text-center"
          style="display: grid; place-items: center"
        >
          <v-img
            src="@/assets/gallery/10_years_free_service.png"
            contain
            width="100%"
            height="250px"
          ></v-img>
        </v-col>
        <v-col order="1" align-self="center" class="text-center"
          ><p class="primary--text  text-h3 font-weight-bold xs-mt-4">
            Jyoti Plumbing Solutions Company
          </p>
          <p class="text-subtitle-2 secondary--text ">For all your plumbing needs call us at +91 9646196562</p></v-col
        >
      </v-row>
      <circle-cards></circle-cards>
      <cards-description></cards-description>
      <our-brands></our-brands>
      <our-location></our-location>
    </v-container>
  </div>
</template>

<script>
import CardsDescription from "@/components/CardsDescription.vue";
// import PhotoGallery from '@/components/PhotoGallery.vue';
import OurBrands from "@/components/OurBrands.vue";
import OurLocation from "@/components/OurLocation.vue";
import CircleCards from "@/components/CircleCards.vue";
export default {
  components: {
    CardsDescription,
    OurBrands,
    OurLocation,
    CircleCards,
  },
  metaInfo: {
    titleTemplate: "Home - Jyoti Plumbing Solutions",
    meta: [
      {
        name: "description",
        content:
          "Jyoti Plumbing Solutions provide 10 years free service guarantee for new house projects. Our services are 100% percent guaranteed for any kind of leaks. ",
      },
      {
        name: "keywords",
        content:
          "best plumbing services, 100% service guarantee, plumber in devigarh, plumber in naneola, plumber in patiala",
      },
    ],
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
