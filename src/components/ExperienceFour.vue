<template>
  <section class="experience-four">
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
  name: "ExperienceFour",
  data() {
    return {
      experience: {
        company: "Breslaw Plumbing LLC",
        role: "Administrative Manager",
        location: "NYC",
        website: "www.breslawplumbing.com",
        period: "start - end",
        descriptions: [
          "Provided day-to-day administrative management, supervision and coordination of construction activities.",
          "Assisted project managers with creating and communicating project timelines, and processing constructions drawings using AutoCAD.",
          "Initiated and implemented a cutting edge cloud computing solution for managing constructions projects which drastically improved communication and productivity."
        ]
      }
    };
  }
};
</script>

