<template>
  <section class="experience-four text-sm mb-4">
    <div></div>
    <div class="flex flex-wrap">
      <div class="company font-semibold mr-2">{{experience.company}}- </div>
      <div class="role mr-2 font-thin">{{experience.role}}- </div>
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
  name: "ExperienceFour",
  data() {
    return {
      experience: {
        company: "Breslaw Plumbing LLC",
        role: "Administrative Manager",
        location: "NYC",
        website: "www.breslawplumbing.com",
        period: "Jun 2008 - Jul 2011",
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

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
}
</style>
