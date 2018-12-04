<template>
  <section class="experience-three mb-4 text-sm">
    <div></div>
    <div class="flex flex-wrap">
      <div class="company font-semibold mr-2">{{experience.company}} -</div>
      <div class="role mr-2 font-thin">{{experience.role}} -</div>
      <div class="location font-thin">{{experience.location}}</div>
      <div class="period font-thin ml-auto">{{experience.period}}</div>
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
  name: "ExperienceThree",
  data() {
    return {
      experience: {
        company: "Kira Farms",
        role: "Technical Project Manager",
        location: "Lagos, Nigeria",
        period: "Nov 2011 – Jan 2013",
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


<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
  grid-gap: 10px;
}
</style>