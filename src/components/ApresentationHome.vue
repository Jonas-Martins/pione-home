<template>
  <v-row class="justify-center">
    <v-col class="d-flex flex-column justify-center align-center" cols="5">
      <b>
        <span style="font-size: 3.5rem; line-height: 120%; ">
          Buy, Sell & Swap Digital Assets<span style="color: purple">.</span>
        </span>
      </b>
      <span style="text-align: justify">
        Order prices are locked in at the time of placement and our
        non-custodial approach allows for complete control of your Assets
        <br />
        <b>Place on order in 5 minutes!</b>
      </span>
      <div class="mt-16 d-flex justify-center">
        <v-btn class="mx-5" color="purple" dark large> Get Started </v-btn>
        <v-btn
          class="mx-5"
          color="purple"
          text
          large
          style="text-decoration: underline"
        >
          How it Works
        </v-btn>
      </div>
    </v-col>
    <v-col style="height: 100%" cols="5" class="d-flex justify-end">
      <img
        height="100%"
        width="100%"
        :src="require(`@/assets/characters/charHome/homeChar${randomImg}.svg`)"
      />
    </v-col>
  </v-row>
</template>

<script>
export default {
  computed: {
    randomImg() {
      return Math.floor(Math.random() * (6 - 1) + 1);
    },
  },
};
</script>

<style scoped>
</style>

