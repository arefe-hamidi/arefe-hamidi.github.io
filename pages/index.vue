<template>
  <div>
    <b-container>
      <PersonalInfo />
      <Summary />
    </b-container>
  </div>
</template>

<script>
import Summary from "../components/Summary.vue";
import PersonalInfo from "../components/PersonalInfo.vue";
export default {
  name: "IndexPage",
  components: {
    Summary,
    PersonalInfo,
  },
};
</script>
