<template>
    <v-card
      class="mx-auto overflow-visible"
      width="400"
      height="480"
      style="background: #5eb4e2; color: #fff"
    >
      <div class="d-flex justify-space-between pa-2">
        <h1 style="color: #000">About</h1>
        <NuxtLink @click="goToAbout"
          ><v-icon size="60">mdi-home</v-icon></NuxtLink
        >
      </div>
      <div class="d-flex justify-center align-center">
        <v-icon
          style="border-radius: 25px; background: #fff; color: #6c6666"
          size="200"
          icon="mdi-account"
        ></v-icon>
      </div>
      <div class="overflow-visible pa-4">
        <p  style="color: #000000">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium
          dolore consequatur voluptates odio vel quae deleniti magni earum quia
          quam omnis, voluptatibus aliquid inventore iusto nesciunt maiores in
          suscipit. Perferendis. Lorem ipsum dolor sit amet, consectetur
          adipisicing elit. Accusantium dolore consequatur voluptates odio vel
          quae deleniti magni earum quia quam omnis, voluptatibus aliquid
          inventore iusto nesciunt maiores in suscipit. Perferendis.
        </p>
      </div>
    </v-card>
  </template>
  
  <script>
  export default {
    name: "About",
  };
  </script>
  
  <style lang="scss" scoped>
  .text-h4 h4 {
    color: #000;
    font-weight: bold;
  }
  .about-icon {
    width: 300px;
    height: 250px;
    margin: auto;
    background: #fff;
  }
  </style>