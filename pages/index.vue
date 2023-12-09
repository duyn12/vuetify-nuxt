<template>
  <div>
    <div class="section_menu">>
      <v-card
      width="250"
      height="250"
      class="box-1 d-flex justify-center align-center"
    >
      <v-card-item>
        <div class="text-h3">
          <NuxtLink @click="goToHome"> Home </NuxtLink>
        </div>
      </v-card-item>
    </v-card>
    <v-card
      width="250"
      height="250"
      class="box-2 d-flex justify-center align-center"
    >
      <v-card-item>
        <div class="text-h3">
          <NuxtLink @click="goToAbout"> About </NuxtLink>
        </div>
      </v-card-item>
    </v-card>
    <v-card
      width="250"
      height="250"
      class="box-3 d-flex justify-center align-center rounded-circle"
    >
      <v-card-item>
        <div class="text-h3">
          <NuxtLink @click="goToInfo"> Info </NuxtLink>
        </div>
      </v-card-item>
    </v-card>
    </div>
    <div class="container">
      <form class="form">
        <input placeholder="Name" class="input" type="text" />
        <input placeholder="Password" class="input" type="password" />
        <button class="btn">Login</button>
      </form>
  </div>
  </div>

</template>

<script>
export default {
  name: "Home",
  methods: {
    goToHome() {
      console.log("click Home");
    },
    goToInfo() {
        console.log("Info");
        setTimeout(() => {
        this.$router.push("/info");
        // Hiển thị thông báo "Exit page" 
        setTimeout(() => {
          console.log("Exit page");
        }, 2000);
      }, 15000);
    },
    goToAbout() {
      console.log("Info");
        setTimeout(() => {
        this.$router.push("/about");
        setTimeout(() => {
          console.log("Exit page");
        }, 2000);
      }, 15000);
    },
  },
};
</script>

<style scoped>
.section_menu {
  position: relative;
  width: 100%;
  height: 450px;
}
.container {
  width: 100%;
}
.box-1 {
  position: absolute;
  left: 30%;
  top: 16%;
  background: rgb(112, 179, 255);
}
.box-2 {
  position: absolute;
  top: 35%;
  left: 44%;
  background: yellow;
}
.box-3 {
  position: absolute;
  top: 15%;
  left: 58%;
  background: red;
}
a {
  text-decoration: none;
}
.text-h3 {
  cursor: pointer;
}
.form {
  margin: 0 auto;
  width: 450px;
  display: flex;
  flex-direction: column;
  gap: 10px;
  padding-top: 3em;
  padding-left: 2.8em;
  padding-right: 2.8em;
  padding-bottom: 2.1em;
  border-radius: 35px;
  background-color: #22b9df;
  transition: 0.4s ease-in-out;
}
::placeholder {
  color: #000000;
  text-align: center;
  font-weight: bold;
}
.form .input {
  outline: none;
  padding: 0.5em;
  color: #000000;
  border-radius: 35px;
  background-color: #ffffff;
  text-align: center;
}
.form .btn {
  align-self: center;
  margin-top: 2em;
  border-radius: 35px;
  border: none;
  color: rgb(0, 0, 0);
  background-color: #0aaf39;
  font-weight: bold;
  transition: 0.4s ease-in-out opacity, 0.1s ease-in-out active;
  padding: 10px;
  width: 350px;
}
</style>
