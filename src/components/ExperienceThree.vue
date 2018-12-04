<template>
  <section class="experience-three">
    <div>Experience</div>
    <div>
      <div class="company">{{experience.company}}</div>
      <div class="role">{{experience.role}}</div>
      <div class="period">{{experience.period}}</div>
    </div>
    <ul>
      <li
        class="description"
        v-for="n in experience.descriptions"
        :key="n.company"
      >{{n}}</li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "ExperienceThree",
  data() {
    return {
      experience: {
        company: "Kira Farms",
        role: "Technical Project Manager",
        location: "Lagos, Nigeria",
        website: "www.kirafarms.com",
        period: "start - end",
        descriptions: [
          "Coordinated the planning, budgeting, and scheduling of hardware procurement and - development of 5- acre Greenhouse farm.",
          "Developed strategies to achieve objectives in implementation and execution of the project."
        ]
      }
    };
  }
};
</script>

