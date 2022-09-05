<template>
  <nav class="d-flex justify-space-around align-center">
    <div>
      <img width="50px" src="@/assets/logos/Pione2Dark.svg" />
    </div>
    <div>
      <ul class="d-flex" style="list-style: none; color: black">
        <li
          style="cursor: pointer; font-size: large"
          class="mx-5"
          v-for="(list, i) in menuList"
          :key="i"
        >
          {{ list.name }}
        </li>
      </ul>
    </div>
    <div>
      <v-btn color="black" dark large> Get Started </v-btn>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      menuList: [
        { name: "Home", link: "" },
        { name: "About", link: "" },
        { name: "Price", link: "" },
        { name: "Contact", link: "" },
        { name: "Jobs", link: "" },
      ],
    };
  },
};
</script>

<style scoped>
</style>>
