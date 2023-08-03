<template>
  <div>
    <b-container>
      <PersonalInfo class="my-2" />
      <Summary class="my-2" />
      <Experiance class="my-2" />
      <Educations class="my-2" />
      <Hobby class="my-2" />
      <Skills class="my-2 mt-4" />
      <Projects class="my-2" />
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
