<template>

  <div class="container mx-auto bg-grey-lighter">
    <Header />
    <ExperienceOne />
    <ExperienceTwo />
    <ExperienceThree />
    <ExperienceFour />
    <ExperienceFive />
    <ExperienceSix />
    <Education />
    <Certificates />
    <Skills />
    <Portfolio />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ExperienceOne from "./components/ExperienceOne.vue";
import ExperienceTwo from "./components/ExperienceTwo.vue";
import ExperienceThree from "./components/ExperienceThree.vue";
import ExperienceFour from "./components/ExperienceFour.vue";
import ExperienceFive from "./components/ExperienceFive.vue";
import ExperienceSix from "./components/ExperienceSix.vue";
import Education from "./components/Education.vue";
import Certificates from "./components/Certificates.vue";
import Skills from "./components/Skills.vue";
import Portfolio from "./components/Portfolio.vue";

export default {
  name: "app",
  components: {
    Header,
    ExperienceOne,
    ExperienceTwo,
    ExperienceThree,
    ExperienceFour,
    ExperienceFive,
    ExperienceSix,
    Education,
    Certificates,
    Skills,
    Portfolio
  }
};
</script>

<style>
</style>
