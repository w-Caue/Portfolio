<script>
import TheHeader from "./components/TheHeader.vue";
import AboutMe from "./components/AboutMe.vue";
import MyProjects from "./components/MyProjects.vue";
import TheFooter from "./components/TheFooter.vue";
import MySkills from "./components/MySkills.vue";
import WhyChooseMe from "./components/WhyChooseMe.vue";
import TheContact from "./components/TheContact.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    AboutMe,
    MySkills,
    MyProjects,
    WhyChooseMe,
    TheContact,
    TheFooter
  },
};
</script>

<template>
  <TheHeader />
  <AboutMe />
  <MySkills/>
  <MyProjects />
  <WhyChooseMe />
  <TheContact />
  <TheFooter />

  
</template>

<style>
#app {
  text-align: center;
  color: #2c3e50;
  /* background-color:#C0DFFC; */
}
</style>
