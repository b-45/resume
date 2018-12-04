<template>
  <section class="experience-one">
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
  name: "ExperienceOne",
  data() {
    return {
      experience: {
        company: "Almat Group",
        role: "Associate",
        location: "NYC",
        period: "start - end",
        descriptions: [
          "Assisted managing partners with all aspects of real estate development transactions.",
          "Managed early-stage and late-stage development activity of construction projects in NYC and emerging markets.",
          "Monitored construction to ensure compliance with contract documents and scope of work.",
          "Developed presentations and leverage data-driven insights to direct acquisition strategy of new opportunities."
        ]
      }
    };
  }
};
</script>

