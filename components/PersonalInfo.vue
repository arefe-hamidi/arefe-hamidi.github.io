<template>
  <div class="personal-info my-3">
    <div class="d-flex flex-row">
      <div class="d-flex flex-row">
        <div>
          <img :src="ImageSrc" class="profile-image" />
        </div>
        <div class="mx-3">
          <div>
            <h1 class="importent-title">Front-End Developer</h1>
          </div>
          <div>
            <h3 class="title">Arefeh Hamidi</h3>
          </div>
          <hr />
          <div>
            <label for="" class="info-label">DoB:</label>
            <span class="info-detail"> 1997-02-26</span>
          </div>
          <div>
            <label for="" class="info-label">Marital Status:</label>
            <span class="info-detail"> Married</span>
          </div>
        </div>
      </div>
      <div class="d-flex flex-column justify-content-center ml-auto">
        <div>
          <img src="~/assets/icon/envelope-solid.svg" class="icon" alt="" />
          <span class="info-detail"> arefehamidi.guilan@gmail.com</span>
        </div>
        <div>
          <img src="~/assets/icon/phone-solid.svg" class="icon" alt="" />
          <span class="info-detail"> (+98)9112333453</span>
        </div>
        <div>
          <img src="~/assets/icon/location-dot-solid.svg" class="icon" alt="" />
          <span class="info-detail"> Rasht, Iran</span>
        </div>
        <div>
          <img src="~/assets/icon/linkedin.svg" class="icon" alt="" />
          <span class="info-detail">
            <a
              href="https://www.linkedin.com/in/arefe-hamidi-87a440168/"
              class="link-text"
              >Arefe Hamidi
            </a>
          </span>
        </div>
        <div>
          <img src="~/assets/icon/github.svg" class="icon" alt="" />
          <span class="info-detail">
            <a href="https://github.com/arefe-hamidi" class="link-text"
              >arefe-hamidi</a
            ></span
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ImageSrc: require("~/assets/images/profileImage.jpeg"),
    };
  },
};
</script>

<style lang="css" scoped>
.profile-image {
  height: 200px;
  width: 200px;
  border-radius: 50%;
  border: 4px solid #bed3d6;
}
</style>
