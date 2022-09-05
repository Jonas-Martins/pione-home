<template>
  <footer>
    <div
      class="d-flex justify-center align-center flex-column"
      style="height: 45%"
    >
      <span style="color: white; font-size: 40px; font-weight: 600"
        >Let´s keep in touch!</span
      >
      <div class="d-flex justify-center align-center mt-5" style="color: white">
        <v-chip color="white" @click="true" class="mx-4"
          ><v-icon color="blue" class="mr-2">mdi-facebook</v-icon>
          Facebook</v-chip
        >
        <v-chip color="white" @click="true" class="mx-4"
          ><v-icon color="pink" class="mr-2">mdi-instagram</v-icon>
          Instagram</v-chip
        >
        <v-chip color="white" @click="true" class="mx-4"
          ><v-icon color="red" class="mr-2">mdi-youtube</v-icon> Youtube</v-chip
        >
        <v-chip color="white" @click="true" class="mx-4"
          ><v-icon color="blue" class="mr-2">mdi-twitter</v-icon>
          Twitter</v-chip
        >
        <v-chip color="white" @click="true" class="mx-4"
          ><v-icon color="green" class="mr-2">mdi-whatsapp</v-icon>
          Whatsapp</v-chip
        >
      </div>
    </div>
    <div>
      <v-row class="rigths ma-0" justify="center">
        <v-col cols="4">
          <h1>Pione</h1>
          <v-text-field 
            class="mt-16"
            label="Subscribe to our newsletter!"
            placeholder="your@email.com"
            filled
            rounded
            dense
            prepend-inner-icon="mdi-email"
            append-icon="mdi-send"
            color="white"
            background-color="#9c27b0a1"
            style="width: 80%"
            dark
          ></v-text-field>
        </v-col>
        <v-col cols="3">
          <b>Navegation</b>
          <ul style="list-style: none" class="mt-6">
            <li class="ml-n6" v-for="(list, i) in menuList" :key="i">
              <span style="cursor: pointer">{{ list.name }}</span>
            </li>
          </ul>
        </v-col>
        <v-col cols="3" class="d-flex flex-column">
          <b>Connect with us</b>
          <span class="mt-5">contact@pione.com.br</span>
          <span>(+55) 15 98837-1251</span>
        </v-col>
        <v-col cols="12" class="d-flex justify-center">
          <span>© 2022 Pione - Todos os direitos reservados.</span>
        </v-col>
      </v-row>
    </div>
  </footer>
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
footer {
  background-image: url(@/assets/characters/backAnimate6.svg);
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  background-position-y: 45%;
}
.rigths {
  mix-blend-mode: difference;
  color: purple;
}
</style>