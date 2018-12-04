<template>

  <div class="container mx-auto bg-grey-lighter">
    <Header></Header>
    <ExperienceOne></ExperienceOne>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ExperienceOne from "./components/ExperienceOne.vue";

export default {
  name: "app",
  components: {
    Header,
    ExperienceOne
  }
};
</script>

<style>
</style>
