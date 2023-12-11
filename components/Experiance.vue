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
          <div class="info-detail">
            <span>
              {{ work.companyName }} - {{ work.EmploymentType }} (
              {{ work.locationType }})</span
            >
            <!-- <span>
              <img
                src="~/assets/icon/location-dot-solid.svg"
                class="icon"
                alt=""
              />
              {{ work.location }} - {{ work.EmploymentType }} -
              {{ work.locationType }}</span
            > -->
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
          jobPosition: "Front-end developer",
          companyName: "Rayka",
          EmploymentType: "Full time",
          startDate: "Aug 2023",
          endDate: "Now",
          locationType: "Remote",
          location: "Rasht, Guilan Province, Iran",
          achievements: [
            "Designed   front-end   code   using   React.js   with TypeScript   to   develop   responsive   website that work across desktop, tablets, and other devices.",
            "Created   modular   templates   using   modern CSS techniques and JavaScript libraries.",
          ],
        },
        {
          jobPosition: "Team leader of front-end team",
          companyName: "Nasr Moein Parsayan",
          EmploymentType: "Full time",
          endDate: "Jul 2023",
          startDate: "Apr 2022",
          locationType: "Remote",
          location: "Tehran, Tehran Province, Iran",
          achievements: [
            "Mentored a team of 4 members, facilitating their professional growth and helping them achieve personal goals .",
            "Worked on projects involving <<payment gateway>> integration, including payment processing, wallet charging, subscription, and membership plans.",
            "Optimized 15+ key content pages for <<SEO>> objectives, resulting in a 78% improvement in online search ranking accuracy (utilized <<SSR>>, <<CSR>>, <<SPA>>, <<sitemap>>, <<meta tags>>, etc.).",
            "Conducted code reviews to improve product quality.",
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
            "Designed front-end code using Vue.js and Nuxt.js to develop responsive websites that work across desktop, tablets, and other devices.",
            "Fixed bugs and performed code reviews, utilizing the module pattern architecture within the first month.",
            "Created modular, responsive templates using modern CSS techniques and JavaScript libraries.",
            "Collaborated with designers to ensure efficient and technically sound designs",
            "Optimized 18+ applications for maximum speed and scalability.",
            "Utilized <<Leaflet>>, <<CKEditor>>, <<Vuex>>, <<Sass>>, and other tools in the projects.",
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
            "Designed front-end code using Vue.js and Nuxt.js to develop responsive websites.",
            "Utilized <<D3.js>> to create a tree structure for managing menus in the admin panel.",
            "Validated 100% of user input before submitting it to the back-end.",
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
