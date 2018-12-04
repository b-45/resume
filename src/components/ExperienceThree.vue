<template>
  <section class="experience-three">
    <div>Experience</div>
    <div>
      <div class="company">{{experience.company}}</div>
      <div class="role">{{experience.role}}</div>
      <div class="location">{{experience.location}}</div>
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
        period: "start - end",
        descriptions: [
          "Assisted founders with implementation approach and deployment strategy for 5-acre Greenhouse farm.",
          "Working with local and international stakeholders to organize various activities necessary to coordinated planning, procure hardware, labor and other resources.",
          "Developed strategies to achieve objectives in implementation and execution of the project."
        ]
      }
    };
  }
};
</script>

