<script>
import TheHeader from "./components/TheHeader.vue";
import AboutMe from "./components/AboutMe.vue";
import MyProjects from "./components/MyProjects.vue";
import TheContact from "./components/TheContact.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    AboutMe,
    MyProjects,
    TheContact,
    TheFooter
  },
};
</script>

<template>
  <TheHeader />
  <AboutMe />
  <MyProjects />
  <TheContact />
  <TheFooter />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* background-color:#C0DFFC; */
}
</style>
