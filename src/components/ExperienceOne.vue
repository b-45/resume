<template>

  <section class="experience-one mb-4 text-sm">
    <div class="font-semibold">Experience</div>
    <div class="flex flex-wrap">
      <div class="company font-semibold mr-2">{{experience.company}} - </div>
      <div class="role mr-2 font-thin">{{experience.role}} -</div>
      <div class="location">{{experience.location}}</div>
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
  name: "ExperienceOne",
  data() {
    return {
      experience: {
        company: "Almat Group",
        role: "Associate",
        location: "NYC",
        period: "Nov 2015 – Present",
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

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
}
</style>
