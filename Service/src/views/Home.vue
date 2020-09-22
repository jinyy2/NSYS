<template>
  <v-row
      align="center"
      justify="center"
  >
    <v-col cols="12">
      <v-hover
          v-slot:default="{ hover }"
      >
        <v-card
            :elevation="hover ? 12 : 2"
            class="mx-auto"
            height="350"
            max-width="350"
        >
          <v-img
              src="https://cdn.vuetifyjs.com/images/cards/kitchen.png"
              height="200px"
          ></v-img>
          <v-card-text class="my-4 text-center title">Hover over me!</v-card-text>
          <v-img
              src= "@/assets/insertcoin.png"
              height="200px"
          ></v-img>
        </v-card>
      </v-hover>
      <h1>----</h1>
      <coin></coin>
    </v-col>
  </v-row>
</template>

<script>
import { mapState, mapGetters } from 'vuex'
import coin from '@/components/Main.vue'
import img from '@/assets/insertcoin.png'
  export default {
  components:{
    coin
  },
    data() {
      return {
        img
      }
    },
    computed:{
      ...mapGetters({
          count: 'allUsersCount',
          seouls : 'countOfSeoul',
          percent : 'percentOfSeoul'
        },
      )
    }
  }
</script>