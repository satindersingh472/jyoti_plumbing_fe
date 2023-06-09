<template>
    <div>
        <v-app-bar-nav-icon @click="drawer = !drawer" ></v-app-bar-nav-icon>
        <v-navigation-drawer
      v-model="drawer"
        right
        absolute
        temporary
        height="50vh"
    >
      <v-list
      >
        <v-list-item-group
          v-model="group"
          class="text-body-1"
        >
          <v-list-item>
            <v-list-item-title>Contact</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Location</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    </div>
</template>

<script>
    export default {
        data() {
            return {
                drawer: false,
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>