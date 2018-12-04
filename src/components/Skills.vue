<template>
  <section class="skills text-sm mb-4">
    <div class="font-semibold">Skills</div>
    <div>
      SQL,
      HTML,
      CSS,
      Javascript,
      Vue.Js,
      Python,
      Node.js,
      R,
      Tidyverse,
      Tableau,
      Microsoft Office,
      Kanban,
      Kaizen,
      SCRUM,
      Agile
    </div>
  </section>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      skills: []
    };
  }
};
</script>

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
}
</style>

