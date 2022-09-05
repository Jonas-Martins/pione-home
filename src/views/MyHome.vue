<template>
  <div style="height: 100vh;">
    <div class="apresentationBack">
        <TopMenu style="height: 13%"></TopMenu>
        <ApresentationHome style="height: 90%"></ApresentationHome>
    </div>
    <AboutHome style="height: 100%"></AboutHome>
    <FooterHome style="height: 100%;"></FooterHome>
  </div>
</template>

<script>
import TopMenu from "@/components/TopMenu.vue";
import ApresentationHome from "@/components/ApresentationHome.vue";
import AboutHome from "@/components/AboutHome.vue";
import FooterHome from "@/components/FooterHome.vue";
export default {
  components: {
    TopMenu,
    ApresentationHome,
    AboutHome,
    FooterHome
  },
};
</script>

<style>
.apresentationBack {
  background-image: url(@/assets/characters/backAnimate3.svg);
  height: 100%;
  width: 100%;
  background-repeat:round;
  position: relative;
}
</style>