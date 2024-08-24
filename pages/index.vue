<template>
  <div>
    <b-container>
      <PersonalInfo class="mb-2" />
      <b-row>
        <b-col md="9">
          <Summary class="mb-2" />
          <Experiance class="mb-2" />
          <Educations class="mb-2" />
          <!-- <Hobby class="my-2" /> -->
        </b-col>
        <b-col md="3">
          <Skills class="mb-2" />
          <Projects class="mb-2" />
        </b-col>
      </b-row>
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
