<template>
  <div>
    <v-container class="grid mt-5">
      <v-row no-gutters justify="center">
        <v-col align-self="center" cols="12" md="6">
          <p  class="primary--text text-h4 text-md-h3">Reasons To Choose Us</p>
          <p class="primary--text font-weight-bold">
            You can rely on our experienced and educated employees
          </p>
          <p class="secondary--text">
            Our experienced team is always ready to provide the best customer
            service. We are quicker, reliable and trustworthy. We offer 24/7
            emergency services, affordable prices by working from multiple
            branches to help serve our customers faster and efficient.
          </p>
        </v-col>
        <v-col align-self="center" class="grid" cols="12" md="6">
          <v-list>
            <v-list-item v-for="(item, index) in items" :key="index">
              <v-list-item-icon
                ><v-icon class="primary--text" large>{{
                  item["icon"]
                }}</v-icon></v-list-item-icon
              >
              <v-list-item-content class="secondary--text">{{
                item["name"]
              }}</v-list-item-content>
            </v-list-item>
          </v-list>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          name: "Super Fast Service",
          icon: "mdi-lightning-bolt-circle",
        },
        {
          name: "Excellent Customer Service",
          icon: "mdi-handshake-outline",
        },
        {
          name: "100% Service Guarantee",
          icon: "mdi-check-decagram-outline",
        },
        {
          name: "Affordable Pricing",
          icon: "mdi-currency-rupee",
        },
        {
          name: "Multiple Branches",
          icon: "mdi-store",
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
