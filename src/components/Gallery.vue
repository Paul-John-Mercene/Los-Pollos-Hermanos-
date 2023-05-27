<template>
  <v-container>
    <div class="block galleryBlock">
      <h2 class="text-center"> Gallery </h2>
      <v-row>
        <v-col
          v-for="item in items"
          :key="item.id"
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="item.src"
            aspect-ratio="1"
            class="grey lighten-2"
          >
            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
              >
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
export default {
  name: 'MyGallery',
  data() {
      return{
        items: [
          {
            id: 1,
            src: require("../assets/logo.png")
          },
          {
          id: 2,
          src: require("../assets/logo.png")
          },
          {
          id: 3,
          src: require("../assets/logo.png")
          },
          {
          id: 4,
          src: require("../assets/logo.png")
          },
          {
          id: 5,
          src: require("../assets/logo.png")
          },
          {
          id: 6,
          src: require("../assets/logo.png")
          },
          {
          id: 7,
          src: require("../assets/logo.png")
          },
          {
          id: 8,
          src: require("../assets/logo.png")
          },
          {
          id: 9,
          src: require("../assets/logo.png")
          },
        ]
      }
    }
}
</script>

<style>
.galleryBlock {
  background-color: green;
}
</style>

