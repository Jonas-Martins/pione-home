<template>
  <v-app>
    <MyHome></MyHome>
  </v-app>
</template>

<script>
import MyHome from "./views/MyHome.vue";
export default {
  components: {
    MyHome,
  },
  name: "App",

  data: () => ({
    //
  }),
};
</script>
<style>
* {
  font-family: "Secular One", sans-serif;
}
</style>
