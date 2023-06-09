<template>
  <div>
    <v-container fluid class="fill-height" style="display: grid;place-items:center" >
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
          <p class="primary--text text-h3 font-weight-bold mt-2 mb-4">
            Jyoti Plumbing Solutions Company
          </p>
        </v-col>
      </v-row>
     <cards-description ></cards-description>

     <our-brands></our-brands>
    </v-container>
  </div>
</template>

<script>
import CardsDescription from '@/components/CardsDescription.vue';
// import PhotoGallery from '@/components/PhotoGallery.vue';
import OurBrands from '@/components/OurBrands.vue'
export default {
    components:{
        CardsDescription,
        // PhotoGallery,
        OurBrands,
    },
  metaInfo: {
    titleTemplate: "Home - Jyoti Plumbing Solutions",
    meta: [
      {
        name: "description",
        content:
          "Jyoti Plumbing Solutions provide 10 years free service guarantee for new house projects.",
      },
    ],
  },
  data() {
    return {
      services: [
        {
          name: "Flushing",
          image:
            "https://www.reshot.com/preview-assets/icons/7T9JFBDCAU/toilet-7T9JFBDCAU.svg",
        },
        {
          name: "Fitting",
          image:
            "https://www.reshot.com/preview-assets/icons/T89XN24F7J/water-pipe-T89XN24F7J.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
