<template>
    <v-card class="mx-auto form-info overflow-visible rounded-xl" style="color: #fff">
      <div class="text-h3 d-flex justify-end">
        <NuxtLink @click="goToHome"
          ><v-icon >mdi-home</v-icon></NuxtLink
        >
      </div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium
          dolore consequatur voluptates odio vel quae deleniti magni earum quia
          quam omnis, voluptatibus aliquid inventore iusto nesciunt maiores in
          suscipit. Perferendis. Lorem ipsum dolor sit amet, consectetur
          adipisicing elit. Accusantium dolore consequatur voluptates odio vel
          quae deleniti magni earum quia quam omnis, voluptatibus aliquid
          inventore iusto nesciunt maiores in suscipit. Perferendis.
        </p>
        <div class="text-h1 font-weight-bold d-flex justify-center align-center mt-12">Info</div>
    </v-card>
  </template>
    
  <script>
  export default {
    name: "Info",
  };
  </script>
    
    <style lang="scss" scoped>
  .form-info {
    width: 400px;
    height: 500px;
    padding: 10px 20px;
    background: #ed4f4f;
  }
  .form-info p {
    color: #fff;
  }
  </style>