<template>
  <div class="d-flex justify-center">
    <div style="position: absolute; height: 99vh; width: 100%;">
      <img height="100%" src="@/assets/characters/teste.svg" />
    </div>
    <div style="position: absolute; height: 99vh; width: 100%; z-index: 1;">
      <img height="100%" src="@/assets/characters/teste2.svg" />
    </div>
    <div style="position: absolute; z-index: 999; height: 100vh;">
      <TopMenu style="height: 13%;"></TopMenu>
      <ApresentationHome style="height: 87%;"></ApresentationHome>
    </div>
  </div>
</template>

<script>
import TopMenu from "@/components/TopMenu.vue";
import ApresentationHome from "@/components/ApresentationHome.vue";
export default {
  components: {
    TopMenu,
    ApresentationHome,
  },
};
</script>

<style>
</style>