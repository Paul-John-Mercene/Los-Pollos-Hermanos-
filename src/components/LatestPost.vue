<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Latest Post</h2>
      <v-row>
        <v-col v-for="item in items" :key="item.id" cols="12" md="4">
          <v-card style="background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url(require('@/core/assets/homeBg.png')) center center / cover no-repeat" outlined class="mx-auto">
            <v-img
              class="white--text align-end"
              height="200px"
              :src="item.src"
            >
              <v-card-title>{{ item.title }}</v-card-title>
            </v-img>
            <v-card-subtitle class="pb-0">{{ item.subtitle }}</v-card-subtitle>
            <v-card-text class="text--primary">
              <div>{{ item.description }}</div>
            </v-card-text>
            <v-card-actions>
              <v-btn color="primary" text>More</v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "LatestPost",
  data: () => ({
    show: false,
    items: [
      {
        id: 1,
        title: "Boso-Boso, Antipolo",   
        description: "Boso-Boso, located in Antipolo, is a scenic and tranquil destination that offers a retreat from the bustling city life of Metro Manila, Philippines. ",
        src: require("../assets/images/car4.jpg")
      },
      {
        id: 2,
        title: "Groupings",
        description: "In cooperative learning, students are organized into small groups to work together on tasks or projects. This promotes teamwork.",
        src: require("../assets/images/img1.jpg")
      },
      {
        id: 3,
        title: "Boss Golden Resort",
        description: "Boss Golden Resort, located in Antipolo, is a charming and inviting destination that offers a relaxing getaway from the city's hustle.",
        src: require("../assets/images/boss.jpg")
      }
    ]
  })
};
</script>
