<template>
  <section class="experience-two mb-4 text-sm">
    <div></div>
    <div class="flex flex-wrap">
      <div class="company font-semibold mr-2">{{experience.company}} -</div>
      <div class="role mr-2 font-thin">{{experience.role}} -</div>
      <div class="location font-thin">{{experience.location}}</div>
      <div class="period ml-auto font-thin">{{experience.period}}</div>
      <ul class="mt-1">
        <li
          class="description leading-normal"
          v-for="n in experience.descriptions"
          :key="n.company"
        >{{n}}</li>
      </ul>
    </div>
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
        period: "May 2013 - Sep 2015",
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

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
  grid-gap: 10px;
}
</style>