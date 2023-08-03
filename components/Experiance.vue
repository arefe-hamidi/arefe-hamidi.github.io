<template>
  <div>
    <b-card class="my-2">
      <b-card-title outlined>
        <h4 class="title">Work Experience</h4>
      </b-card-title>
      <b-card-text>
        <div v-for="(work, index) in works" :key="index" class="mt-2">
          <div class="d-flex flex-row">
            <div>
              <h5 class="importent-title">{{ work.jobPosition }}</h5>
            </div>
            <div class="ml-auto">
              <span class="info-detail">
                <img
                  src="~/assets/icon/calendar-days-solid.svg"
                  class="icon mr-1"
                  alt=""
                />{{ work.startDate }} - {{ work.endDate }}
              </span>
            </div>
          </div>
          <span class="title">
            {{ work.companyName }}
          </span>
          <div class="info-detail">
            <span>
              <img
                src="~/assets/icon/location-dot-solid.svg"
                class="icon"
                alt=""
              />
              {{ work.location }} - {{ work.EmploymentType }} -
              {{ work.locationType }}</span
            >
          </div>
          <div
            class="achievement mt-1"
            v-for="(achievement, achIndex) in work.achievements"
            :key="achIndex"
          >
            <img
              src="~/assets/icon/circle-solid.svg"
              class="dot-icon mr-1"
              alt=""
            />
            {{ achievement }}
          </div>
        </div>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      works: [
        {
          jobPosition: "Team leader of front-end team",
          companyName: "Nasr Moein Parsayan",
          EmploymentType: "Full time",
          endDate: "Jul 2023",
          startDate: "Apr 2022",
          locationType: "Remote",
          location: "Tehran, Tehran Province, Iran",
          achievements: [
            "master of front-end team management and use vue and nuxt for the projects.",
            " have experience on working with payment gateway in this project such as wallet charge , payment , subscription, membership plan , ... .",
            "I have some experience on SEO include working with vue meta tags and site map . Also I worked with SSR rendering in site.",
          ],
        },
        {
          jobPosition: "Senior front-end developer",
          companyName: "Nasr Moein Parsayan",
          EmploymentType: "Full time",
          startDate: "Dec 2020 ",
          endDate: "Apr 2022",
          locationType: "Remote",
          location: "Tehran, Tehran Province, Iran",
          achievements: [
            "I have worked with OIDC auth for manage user authentication .",
          ],
        },
        {
          jobPosition: "Front-end developer",
          companyName: "Memarenoo",
          EmploymentType: "Freelance",
          startDate: "Jun 2019",
          endDate: "Nov 2020",
          locationType: "On site",
          location: "Gilan Province, Iran",
          achievements: [
            "I have been working as a freelancer in the front-end team and I used vue and nuxt for projects.",
            "I have worked with D3js to create tree for manage menu in admin panel.",
          ],
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
