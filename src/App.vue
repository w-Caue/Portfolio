<template>
  <TheHeader />
  <WhatDo />
  <MyProjects />
  <AboutMe />
  <MySkills />
  <EducationExperience />
  <TheContact />
  <TheFooter />
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import WhatDo from "./components/WhatDo.vue";
import MyProjects from "./components/MyProjects.vue";
import AboutMe from "./components/AboutMe.vue";
import MySkills from "./components/MySkills.vue";
import EducationExperience from "./components/EducationExperience.vue";
import TheContact from "./components/TheContact.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    WhatDo,
    MyProjects,
    AboutMe,
    MySkills,
    EducationExperience,
    TheContact,
    TheFooter
  },
};
</script>

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
