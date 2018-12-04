<template>

  <div class="container mx-auto bg-grey-lighter">
    <Header />
    <ExperienceOne />
    <ExperienceTwo />
    <ExperienceThree />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ExperienceOne from "./components/ExperienceOne.vue";
import ExperienceTwo from "./components/ExperienceTwo.vue";
import ExperienceThree from "./components/ExperienceThree.vue";

export default {
  name: "app",
  components: {
    Header,
    ExperienceOne,
    ExperienceTwo,
    ExperienceThree
  }
};
</script>

<style>
</style>
