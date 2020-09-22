<template>
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
          height="300"
          width="200"
         src="https://cdn.vuetifyjs.com/images/cards/kitchen.png"
      >
      </v-img>
    </v-card>
  </v-hover>
</template>
<script>


</script>
