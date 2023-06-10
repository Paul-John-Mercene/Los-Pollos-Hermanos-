<template>
    <div class="heroBlock">
      <v-carousel cycle>
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
          :src="item.src"
          reverse-transition="fade-transition"
          transition="fade-transition">
          <v-row
            class="fill-height title hidden-xs-only"
            align="center"
            justify="center"
          >
            <div>{{ item.title }}</div>
          </v-row>
        </v-carousel-item>
      </v-carousel>
    </div>
</template>

<script>
  export default {
    name: 'Hero',

    data () {
      return {
        items: [
          {
            src: require("../assets/images/car1.jpg"),
            title: "LOS"
          },
          {
            src: require("../assets/images/car2.jpg"),
            title: "POLLOS"
          },
          {
            src: require("../assets/images/car3.jpg"),
            title: "HERMANOS"
          },
          {
            src: require("../assets/images/car4.jpg"),
            title: "PHOTOGRAPHY"
          }
        ],
      }
    },
  }
</script>
