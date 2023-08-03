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
          title: "Taksan",
          link: "https://taksaanpre.ir/",
          description: " Iran's industrial market online platform",
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
          title: "Taksan's super admin panel",
          link: "https://superadmin.taksaanpre.ir/",
          description: "",
        },
        {
          title: "Taksan's supplier panel",
          link: "https://supplier.taksaanpre.ir/",
          description: "",
        },
        {
          title: "Memareno",
          link: "https://memareno.com/",
          description: "Home design and decoration guide",
        },
      ],
    };
  },
};
</script>

<style></style>
