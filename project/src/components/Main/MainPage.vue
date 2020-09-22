<template>
  <v-container>
    <div>
      <h1>asdfsd</h1>
      <div class="custom-cursor">
        <h2>dalsjf;asklf</h2>
      </div>
      <h1>ldskafj;l</h1>
    </div>
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
            <v-img src="@/assets/insertcoin.png"
            height="350"
            max width="350"></v-img>
          </v-card>
        </v-hover>
      </v-col>
    </v-row>

  </v-container>
</template>
<script>
export default {
  name: "MainPage",
}
</script>
<style>

</style>
<!--<style>-->
<!--.custom-cursor{-->
<!--  cursor : none;-->
<!--  background-image: url("red.png");-->
<!--}-->


