<template>
  <div>
    <b-card>
      <b-card-title outlined>
        <h4 class="title">Projects</h4>
      </b-card-title>
      <b-card-text>
        <div v-for="(proj, index) in projects" :key="index">
          <img
            src="~/assets/icon/circle-solid.svg"
            class="dot-icon mr-1"
            alt=""
          />
          <a :href="proj.link">
            <span class="title">{{ proj.title }}</span>
          </a>

          <span class="info-detail" v-if="proj.description"
            >( {{ proj.description }} )</span
          >
        </div>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: "Ako Rayan website",
          link: "https://akorayan.netlify.app/",
          description: "Transform What's on your mind into What's in your hand",
        },
        {
          title: "Charm db panel",
          link: "https://charmdb.wingstech.org/",
          description: "Flexible outputs,Seamless collaboration",
        },
        {
          title: "Code in One panel",
          link: "https://code.wingstech.org/",
          description: "Do more with less with code in one",
        },
        {
          title: "Rayka Txp",
          link: "http://194.225.78.198/authentication/sign-in",
          description: "One platform for calc merchants txp",
        },
        {
          title: "Clock App",
          link: "http://45.92.94.113:4173/login",
          description: "Managing your time, team & business",
        },
        {
          title: "Taksan",
          link: "https://taksaanpre.ir/",
          description: "Industrial market online platform",
        },
        {
          title: "Taksan's academy site",
          link: "https://academy.taksaan.ir/",
          description: "",
        },
        {
          title: "Taksan's advertisement site",
          link: "https://agahi.taksaanpre.ir/",
          description: "",
        },
        {
          title: "Taksan's supplier panel",
          link: "https://supplier.taksaanpre.ir/",
          description: "",
        },
      ],
    };
  },
};
</script>

<style></style>
