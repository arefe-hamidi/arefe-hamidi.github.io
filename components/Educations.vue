<template>
  <div>
    <b-card class="my-2">
      <b-card-title outlined>
        <h4 class="title">Education</h4>
      </b-card-title>
      <b-card-text>
        <div v-for="(education, index) in Educations" :key="index" class="mt-2">
          <div class="d-flex flex-row">
            <div>
              <h5 class="importent-title">{{ education.FieldOfStudy }}</h5>
            </div>
            <div class="ml-auto">
              <span class="info-detail">
                <img
                  src="~/assets/icon/calendar-days-solid.svg"
                  class="icon mr-1"
                  alt=""
                />{{ education.startDate }} - {{ education.endDate }}
              </span>
            </div>
          </div>
          <span class="title">
            <img
              src="~/assets/icon/location-dot-solid.svg"
              class="icon"
              alt=""
            />
            {{ education.School }} - {{ education.Location }}
          </span>
        </div>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      Educations: [
        {
          FieldOfStudy: "Bachelor of Computer engineering",
          School: "Guilan university",
          Location: "Rasht, Gilan, Iran",
          endDate: "2020",
          startDate: "2015",
        },
        {
          FieldOfStudy: "Diploma in mathematics ",
          School: "Mostaghim high school",
          Location: "Rasht, Gilan, Iran",
          startDate: "2012 ",
          endDate: "2015",
        },
      ],
    };
  },
};
</script>

<style scoped>
.achievement {
  font-size: 14px;
}
</style>
