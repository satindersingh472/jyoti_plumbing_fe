<template>
  <div>
    <v-container
      fluid
      class="fill-height"
      style="display: grid; place-items: center"
    >
      <v-row justify="center">
        <v-col
          class="mt-2 text-center"
          style="display: grid; place-items: center"
        >
          <v-img
            src="@/assets/gallery/10_years_free_service.png"
            contain
            width="100%"
            height="250px"
          ></v-img>
          <p class="primary--text text-h3 font-weight-bold mt-4">
            Jyoti Plumbing Solutions Company
          </p>
        </v-col>
      </v-row>
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
export default {
  components: {
    CardsDescription,
    OurBrands,
    OurLocation,
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
        name:'keywords',
        content:'best plumbing services, 100% service guarantee, plumber in devigarh, plumber in naneola, plumber in patiala'
      }
    ],
  },
  data() {
    return {
    };
  },
};
</script>

<style lang="scss" scoped></style>
