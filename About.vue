<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/img13.jpg">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <div class="headline">About Us</div>
            </v-container>
          </v-col>
        </v-row>
      </v-img>
    </div>
    <div class="block">
      <v-container>
        <p>Photography is an artistic medium that enables us to unleash our creativity and preserve lasting memories for future generations. It serves as a means to capture the essence of the world surrounding us, encompassing both breathtaking landscapes and intricate details, all while narrating captivating stories through singular images. Irrespective of whether one is a seasoned professional or a novice, the journey of honing this craft is forever exhilarating. It allows for the exploration of diverse lighting techniques, compositions, and approaches, resulting in distinctive and visually arresting photographs. Moreover, photography serves as a means of documenting our world, shedding light on social and political issues, and raising awareness for significant causes. So, seize your camera, embark on an exploratory adventure, and unleash the boundless potential of your creativity.</p>
      </v-container>
    </div>
    <div class="block">
      <v-container>
        <h2 class="text-center">Our Team</h2>
        <v-row>
          <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="12" sm="4">
            <v-card flat tile class="mx-auto">
              <v-img :src="item.src" aspect-ratio="1" class="grey lighten-2"></v-img>
              <v-card-text class="text--primary text-center">
                <div class="title">{{ item.name }}</div>
                <p>{{ item.title }}</p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </v-content>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      items: [
        {
          id: 1,
          src: require("../assets/images/masubay.jpg"),
          name: 'Karl Steven Masubay',
          title: 'Director'
        },
        {
          id: 2,
          src: require("../assets/images/sia.jpg"),
          name: 'Jazzmyl Sia',
          title: 'Photographer'
        },
        {
          id: 3,
          src: require("../assets/images/alagos.jpg"),
          name: 'Daniel Joseph Alagos',
          title: 'Freelancer'
        },
        {
          id: 4,
          src: require("../assets/images/francisco.jpg"),
          name: 'Lance Francisco',
          title: 'Freelancer'
        },
        {
          id: 5,
          src: require("../assets/images/colarat.jpg"),
          name: 'Elizalde Colarat Jr.',
          title: 'Freelancer'
        },
        {
          id: 6,
          src: require("../assets/images/mercene.jpg"),
          name: 'Paul John Mercene',
          title: 'Freelancer'
        }
      ]
    };
  }
};
</script>
