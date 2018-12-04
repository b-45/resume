<template>
  <section class="experience-six mb-4 text-sm">
    <div></div>
    <div class="flex flex-wrap">
      <div class="company font-semibold mr-2">{{experience.company}} -</div>
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
  name: "ExperienceSix",
  data() {
    return {
      experience: {
        company: "JPMorgan Inc",
        role: "Internal Consultant Analyst",
        location: "Newark, DE",
        period: "Mar 2000-Nov 2003",
        descriptions: [
          "Responsible for gathering data, analyzing and documenting business processes andmapping departmental domain knowledge.",
          "Collaborated with department stakeholders to identify changes to processes, systems,technology and incorporate change management activities into all aspects of projects usingsix sigma methodologies.",
          "Created training programs & communication plans to increase user adoption and seamless transition of new hires into departmental functions and processes."
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