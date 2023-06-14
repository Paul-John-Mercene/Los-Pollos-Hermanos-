<template>
    <v-container>
      <v-footer 
      padless
      class="custom-footer"
  >
    <v-card
      flat
      tile
      class="my-custom-color white--text text-center"
    >

      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="white--text pt-0">
        Thank you for visiting our photography website. We are passionate about capturing moments and creating visual stories that leave a lasting impression. Our dedicated team of photographers strives to deliver stunning imagery that reflects the beauty of the world around us. Whether it's landscapes, portraits, or special events, we aim to capture the essence and emotion in every frame. We appreciate your support and interest in our work. Feel free to explore our portfolio and reach out to us for any inquiries or collaborations. Let us preserve your cherished memories and bring your vision to life through the art of photography.
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Los Pollos Photography</strong>
      </v-card-text>
    </v-card>
  </v-footer>
    </v-container>
</template>

<script>
  export default {
    name: 'Footer',

    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>