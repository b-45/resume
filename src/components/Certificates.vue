<template>
  <section class="certificates text-sm mb-4">
    <div class="font-semibold">Certificates</div>
    <div>
      <li
        class="description leading-normal list-reset"
        v-for="cert in certificates"
        :key="cert.id"
      >{{cert}}</li>
    </div>

  </section>
</template>

<script>
export default {
  name: "Certificates",
  data() {
    return {
      certificates: [
        "Statistical Thinking for Data Science and Analytics - EDX",
        "Data Manipulation with DPLYR - Datacamp",
        "Data Visualization with GGPLOT - Datacamp",
        "Introduction to R, Statistical Modeling in R - Datacamp",
        "Introduction to Mathematical Thinking - Coursera"
      ]
    };
  }
};
</script>

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
  grid-gap: 10px;
}
</style>

