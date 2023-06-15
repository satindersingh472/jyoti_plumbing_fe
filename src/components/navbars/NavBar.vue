<template>
  <div>
    <v-app-bar app elevate-on-scroll>
      <v-row no-gutters>
        <v-col cols="4" align-self="center"
          ><v-img
            contain
            src="@/assets/logo.png"
            width="100px"
            height="50px"
            position="center"
          ></v-img
        ></v-col>
        <v-col style="justify-items: end;display: grid;" align-self="center"
          ><desktop-nav-bar v-if="desktop_view === true"></desktop-nav-bar
          ><mobile-nav-bar v-if="desktop_view === false"></mobile-nav-bar
        ></v-col>
      </v-row>
    </v-app-bar>
  </div>
</template>

<script>
import DesktopNavBar from "./DesktopNavBar.vue";
import MobileNavBar from "./MobileNavBar.vue";
export default {
  components: { MobileNavBar, DesktopNavBar },
  methods: {
    /*this logic is for the media queries when width is less than 500 then desktop is false 
    and when width is 500 or more desktop view is true and these conditions will change the html on the page*/
    change_querie() {
      if (document.documentElement.clientWidth < 900) {
        this.desktop_view = false;
      } else if (document.documentElement.clientWidth >= 900) {
        this.desktop_view = true;
      }
    },
  },
  mounted() {
    /*change querie method will get activated on mounting so what ever the size of the screen while opening the page it will be responsive
  window add event listener will act upon resizing the window */
    this.change_querie();
    window.addEventListener(`resize`, this.change_querie);
  },
  data() {
    return {
      desktop_view: false,
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
