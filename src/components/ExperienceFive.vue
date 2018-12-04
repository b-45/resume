<template>
  <section class="experience-five">
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
  name: "ExperienceFive",
  data() {
    return {
      experience: {
        company: "Apple Inc",
        role: "Creative",
        location: "NYC",
        period: "start - end",
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

