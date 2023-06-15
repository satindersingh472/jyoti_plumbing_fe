<template>
  <div>
    <v-row justify="center" class="mt-5">
      <v-col
        cols="10"
        md="5"
        lg="3"
        v-for="(card, index) in cards"
        :key="index"
      >
        <v-card shaped elevation="5" class="grey lighten-2" height="150px">
          <v-card-title
            ><v-icon :class="`${card['color']}--text mr-2`" size="35">{{
              card["icon"]
            }}</v-icon
            >{{ card["title"] }}</v-card-title
          >
          <v-card-text class="text-body-2">{{ card["text"] }}</v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          icon: "mdi-comment-flash",
          color: "primary",
          title: "Quick Response Time",
          text: "Our team of experts stay up-to-date with clients and provide solutions and guidence immediately.",
        },
        {
          icon: "mdi-check-decagram",
          color: "success",
          title: "100% Free Service",
          text: "New customers will enjoy 10 years guaranted free services, in case of an issue with the work done by us.",
        },
        {
          icon: "mdi-draw-pen",
          color: "blue",
          title: "Project Blueprint",
          text: "Customers will get blueprint of project and also the details of material used.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
