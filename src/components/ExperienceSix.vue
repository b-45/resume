<template>
  <section class="experience-six">
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
  name: "ExperienceSix",
  data() {
    return {
      experience: {
        company: "JPMorgan Inc",
        role: "Internal Consultant Analyst",
        location: "Newark, DE",
        period: "start - end",
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

