<template>
  <div>
  <v-card
    flat
    class="mx-auto my-1 elevation-0"
    max-width="374"
    height="90%"
    style="border:1px solid #EEEEEE;border-radius:8px"
  >
    <v-img
      height="250"
      :src="require('@/assets/img/main.webp')"
      :lazy-src="require('@/assets/img/main.webp')"
    ></v-img>

    <v-card-title class="google-font">GDG DevFest Gandhinagar 2019</v-card-title>
    <v-card-text>
      <div class="my-0 subtitle-1 black--text google-font">
        GDG Gandhinagar
      </div>

      <div class="google-font">DevFests are community-led, developer events hosted by GDG chapters around the globe focused on community building and learning about Google’s technologies.</div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>

    <v-card-text class="google-font">
      <div class="subtitle-1 text--primary">28th Setember, Gandhinagar</div>
      <div class="subtitle-2 text--primary">Place, Gandhinagar</div>
      <v-chip-group
        small
      >
        <v-chip href="https://twitter.com/hashtag/devfestGandhinagar" target="_blank">#DevFestGandhinagar</v-chip>
        <v-chip href="https://twitter.com/hashtag/devfest" target="_blank">#DevFest</v-chip>
        <!-- <v-chip small outlined>#GDGGandhinagar</v-chip>
        <v-chip small outlined>#GDGGandhinagar</v-chip> -->
      </v-chip-group>
    </v-card-text>

    <v-card-actions class="text-center px-4 mb-5">
        <!-- <p class="google-font">Registration Comming Soon...</p> -->
      <v-btn
        dark
        href="https://devfestpunjab.page.link/registration"
        target="_blank"
        color="primary"
        aria-label="Registration Button"
      >
        Request for an Invitation 
      </v-btn>
      <!-- <v-btn
        text
        color="deep-purple accent-4"
      >
        Learn More
      </v-btn> -->
    </v-card-actions>
  </v-card>

  <v-flex xs12>
    <v-img
      height="1x50"
      :src="require('@/assets/img/svg/footer.svg')"
      :lazy-src="require('@/assets/img/svg/footer.svg')"
    ></v-img>
  </v-flex>

  </div>
</template>

<script>
  export default {
    data: () => ({
      loading: false,
      selection: 1,
    }),

    methods: {
      reserve () {
        this.loading = true

        setTimeout(() => (this.loading = false), 2000)
      },
    },
  }
</script>
