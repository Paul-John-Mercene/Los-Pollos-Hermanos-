<template>
  
    <div class ="block latestPostBlock">
      <v-container>
      <h2 class="text-center"> Latest Post </h2>
    <v-row>
      <v-col cols="4" v-for="item in items" :key="item.id">
      <v-card outlined
    class="mx-auto"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      v-bind:src="item.src"   >
      <v-card-title>{{item.title}}</v-card-title>
    </v-img>

    <v-card-subtitle class="pb-0">{{ item.subtitle }}
    </v-card-subtitle>

    <v-card-text class="text--primary">
      <div>{{ item.description}}</div>
    </v-card-text>

    <v-card-actions>
      <v-btn
        color="primary"
        text>More</v-btn>

      <v-btn
        color="green"
        text
      >
        Explore
      </v-btn>
    </v-card-actions>
  </v-card>
      </v-col>
  </v-row>
</v-container>
    </div>
</template>

<script>
  export default {
    name: 'MyLatestPost',

    data() {
      return{
        items: [
          {
            id: 1,
            title: "Los Pollos Hermanos",
            subtitle: "About Us",
            description: "This will tell about our group.",
            src: require("../assets/logo.png")
          },
          {
          id: 2,
            title: "Photography",
            subtitle: "Sample Pictures",
            description: "Shows our sample photos.",
            src: require("../assets/logo.png")
          },
          {
          id: 3,
            title: "Members",
            subtitle: "Participants",
            description: "Show the members who made the program.",
            src: require("../assets/logo.png")
          },
        ]
      }
    }
}
</script>
