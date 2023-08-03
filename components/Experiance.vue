<template>
  <div>
    <b-card>
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
            "Mentored a team of 4  members, helping team achieve professional growth and personal goals .",
            "Worked on projects involving <<payment gateway>> such as payment, wallet charge, subscription and membership plan .",
            "Optimazed 15+ key content pages for <<SEO>> objectives ,resulting in an 78% improvement in online search ranking accuracy .",
            "Conducted code rivews to improve product quality.",
            "Provided consulting services to professionals during the development of new websites to ensure accessibility.",
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
            "Fixed bugs and performed code reviews, utilizing the <<module pattern>> architecture within the first month .",
            "Created modular, responsive templates using modern CSS techniques and JavaScript libraries.",
            "Collaborated with designers to ensure designs were efficient and technically sound designs.",
            "Optimized 18+ applications for maximum speed and scalability .",
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
            "Designed front-end code using Vue js and Nuxt js to develope responsive web sites that works accross desktop, tablets and other devices .",
            "Utilized D3js to create tree for manage menu in admin panel.",
            "Validated 100% of user input before submitting to the back-end .",
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
