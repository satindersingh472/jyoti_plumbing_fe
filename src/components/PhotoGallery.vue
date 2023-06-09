<template>
    <div class="mt-10" style="display: grid;place-items:center"  >
      <v-row justify="center" no gutters >
        <v-col
          cols="12"
          md="4"
          class="mt-3"
          v-for="(image, index) in images"
          :key="index"
        >
          <v-img :src="`${image['link']}`" height="300px"></v-img>
        </v-col>
      </v-row>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        images: [
          {
            link: require("@/assets/gallery/body_shower_1.jpeg"),
            alt: "installation of a body shower",
            description:
              "We handle complex plumbing infrastructure. Our attention to detail method helps us gain the trust of our customers.",
          },
          {
            link: require("@/assets/gallery/body_shower_2.jpeg"),
            alt: "installation of a body shower",
          },
        ],
      };
    },
  };
  </script>
  
  <style lang="scss" scoped></style>
  