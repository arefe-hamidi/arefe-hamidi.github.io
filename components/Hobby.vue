<template>
  <div>
    <b-card>
      <b-card-title outlined>
        <h4 class="title">Hobby</h4>
      </b-card-title>
      <b-card-text>
        <div v-for="(hooby, index) in hobbies" :key="index">
          <img
            src="~/assets/icon/circle-solid.svg"
            class="dot-icon mr-1"
            alt=""
          />{{ hooby }}
        </div>
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hobbies: [
        "Admirer of nature and beauty",
        "Interested in art, especially traditional art, and reading books",
        "Painting is my main hobby",
        "Interested in traveling, learning about different cultures, and trying new foods",
      ],
    };
  },
};
</script>

<style></style>
