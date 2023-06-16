<template>
  <div>
    <v-container fluid class="fill-height grid">
      <v-row justify="center" class="my-5">
        <v-col order="2" cols="12" md="6" class="md-mt-2 text-center grid">
          <v-img
            src="@/assets/gallery/new_logo.png"
            contain
            class="logo-image grid"
            position="center"
            width="100%"
            height="300px"
          >
          </v-img
          >
        </v-col>
        <v-col order="1" align-self="center" class="text-center"
          ><p class="primary--text text-h3 font-weight-bold xs-mt-4">
            Jyoti Plumbing Solutions Company
          </p>
          <p class="text-subtitle-2 secondary--text">
            For all your plumbing needs call us at +91 9646196562
          </p></v-col
        >
      </v-row>
      <circle-cards></circle-cards>
      <cards-description></cards-description>
      <our-brands></our-brands>
      <great-reasons></great-reasons>
    </v-container>
  </div>
</template>

<script>
import CardsDescription from "@/components/CardsDescription.vue";
// import PhotoGallery from '@/components/PhotoGallery.vue';
import OurBrands from "@/components/OurBrands.vue";
import CircleCards from "@/components/CircleCards.vue";
import GreatReasons from "@/components/GreatReasons.vue";
export default {
  components: {
    CardsDescription,
    OurBrands,
    CircleCards,
    GreatReasons,
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

<style lang="scss" scoped>
.logo-image {
  opacity: 0.2;
  border:1px dashed gray;
}
.grid {
  display: grid;
  place-items: center;
}
</style>
