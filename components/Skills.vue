<template>
  <div>
    <b-card>
      <b-card-title outlined>
        <h4 class="title">Skills</h4>
      </b-card-title>
      <b-card-text>
        <div v-for="(skills, index) in skillsGroup" :key="index" class="mt-3">
          <div>
            <h5 class="importent-title">{{ skills.Title }}</h5>
          </div>
          <b-row>
            <b-col
              cols="12"
              md="4"
              v-for="(skill, skillIndex) in skills.value"
              :key="skillIndex"
            >
              <div class="d-flex flex-row">
                <div>
                  <img
                    src="~/assets/icon/circle-solid.svg"
                    class="dot-icon mr-1"
                    alt=""
                  />{{ skill.title }}
                </div>
                <!-- <div class="ml-auto info-detail">{{ skill.level }}</div> -->
              </div>
            </b-col>
          </b-row>
        </div>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skillsGroup: [
        {
          Title: "Programming languages",
          value: [
            { title: "JavaScript", level: "Proficient" },
            { title: "HTML", level: "Proficient" },
            { title: "CSS", level: "Proficient" },
            { title: "Java", level: "Upper Intermediate" },
            { title: "Python", level: "Intermediate" },
            { title: "Dart", level: "Intermediate" },
            { title: "C++", level: "Intermediate" },
          ],
        },
        {
          Title: "Libraries",
          value: [
            { title: "React", level: "Upper Intermediate" },
            { title: "Redux", level: "Upper Intermediate" },
            { title: "Vuex", level: "Proficient" },
          ],
        },
        {
          Title: "Frameworks",
          value: [
            { title: "Vue js", level: "Proficient" },
            { title: "Next js", level: "Intermediate" },
            { title: "React native ", level: "Intermediate" },
            { title: "Nuxt js", level: "Proficient" },
            { title: "Vuetify", level: "Proficient" },
            { title: "Bootstrap", level: "Proficient" },
            { title: "Flutter", level: "Intermediate" },
          ],
        },
        {
          Title: "Other skills",
          value: [
            { title: "SEO", level: "Upper Intermediate" },
            { title: "Git ", level: "Upper Intermediate" },
            { title: "MySQL", level: "Intermediate" },
            { title: "Adobe illustrator", level: "Intermediate" },
          ],
        },
        {
          Title: "Languages",
          value: [
            { title: "English", level: " Intermediate" },
            { title: "Persian ", level: "Native" },
          ],
        },
      ],
    };
  },
};
</script>

<style></style>
