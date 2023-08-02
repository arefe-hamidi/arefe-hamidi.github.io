<template>
  <div>
    <b-container>
      <PersonalInfo />
      <Summary />
      <Experiance />
      <Educations />
      <Skills />
      <Hobby />
      <Projects />
    </b-container>
  </div>
</template>

<script>
import Summary from "../components/Summary.vue";
import PersonalInfo from "../components/PersonalInfo.vue";
import Educations from "../components/Educations.vue";
import Skills from "../components/Skills.vue";
import Experiance from "../components/Experiance.vue";
import Hobby from "../components/Hobby.vue";
import Projects from "../components/Projects.vue";
export default {
  name: "IndexPage",
  components: {
    Summary,
    PersonalInfo,
    Educations,
    Skills,
    Experiance,
    Hobby,
    Projects,
  },
};
</script>
