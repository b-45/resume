<template>
  <section class="experience-two">
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
  name: "ExperienceTwo",
  data() {
    return {
      experience: {
        company: "Duggal Visual Solutions",
        role: "Project Manager",
        location: "NYC",
        period: "start - end",
        descriptions: [
          "Oversee production planning of custom digital fabrications, installations and rollout of projects ($500K+) for fortune 500 brands.",
          "Liaised and managed communications with stakeholders and engineering team(s) to tease out implementation details, and effectively manage through roadblocks",
          "Developed data products and KPI’s for tracking team performance.",
          "Assisted Creative Director with planning and steering of product development."
        ]
      }
    };
  }
};
</script>

