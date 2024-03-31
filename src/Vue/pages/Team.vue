<template>
  <section id="team" class="light-section">
    <div class="container-fluid">
      <h1 class="section-header">{{ heading }}</h1>
        <div
          v-for="person in people"
          :key="person.name"
          style="display: flex; flex-direction: column; padding-left: 40vw;"
          data-aos="fade-right"
          data-aos-duration="1000"
        >
          <div style="display: flex; align-items: center; margin-bottom: 20px;">
            <img :src="person.flag" width="40" height="40"/>
            <div style="margin-left: 10%;">
              {{ person.name }}
            </div>
  
          </div>
        </div>
      </div>
    <Arrow />
  </section>
</template>

<script>
import data from "../../data/data.json";
import Arrow from "../components/Arrow.vue";

export default {
  name: "Team",
  props: {},
  components: {
    Arrow,
  },
  data() {
    return {
      skills: data.skills.categories,
      heading: data.main.headings.skills,
      currentCategory: data.skills.defaultCategory,
      people: data.skills.people,
    };
  },
  computed: {
    filteredSkills() {
      var skills = data.skills.categories;
      var category = this.currentCategory;
      var filtered = skills.filter(function(x) {
        if (x.category === category) {
          return x;
        }
      });

      console.log(filtered);

      return filtered;
    },
  },
  methods: {
    setCategory(event) {
      this.currentCategory = event.target.dataset.category;
    },
  },
};
</script>

<style lang="scss"></style>
