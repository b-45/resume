<template>
  <section class="certificates">
    <div>Certificates</div>
    <ul>
      <li
        class="description"
        v-for="cert in certificates"
        :key="cert.id"
      >{{cert}}</li>
    </ul>
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

