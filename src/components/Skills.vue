<template>
  <section class="skills">
    <div>Skills</div>
    <ul>
      <li
        class="description"
        v-for="skill in skills"
        :key="skill.id"
      >{{skill}}</li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      skills: [
        "SQL",
        "HTML",
        "CSS",
        "Javascript",
        "Vue.Js",
        "Python",
        "Node.js",
        "R",
        "Tidyverse",
        "Tableau",
        "Microsoft Office",
        "Kanban",
        "Kaizen",
        "SCRUM",
        "Agile"
      ]
    };
  }
};
</script>

