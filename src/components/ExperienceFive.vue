<template>
  <section class="experience-five mb-4 text-sm">
    <div></div>
    <div class="flex flex-wrap">
      <div class="company  font-semibold mr-2">{{experience.company}} -</div>
      <div class="role  mr-2 font-thin">{{experience.role}} -</div>
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
  name: "ExperienceFive",
  data() {
    return {
      experience: {
        company: "Apple Inc",
        role: "Creative",
        location: "NYC",
        period: "Nov 2007 - May 2008",
        descriptions: [
          "Designed and developed technical hands-on training to Apple customers.",
          "Conducted presentations and workshops utilizing Apple's training techniques.",
          "Delivered advanced technical training of audio recording using Logic Audio software."
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
