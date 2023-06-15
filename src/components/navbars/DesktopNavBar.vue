<template>
  <div>
    <v-container class="grid">
      <v-row>
        <v-col align-self="center" v-for="(link, index) in links" :key="index">
          <p class="indigo--text text-h6 ma-0 font-weight-regular">{{ link["name"] }}</p>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          name: "Residential",
        },
        {
            name:'Commercial'
        },
        {
            name:'Emergency'
        },
        {
          name: "Contact",
        },
        {
          name: "Location",
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
