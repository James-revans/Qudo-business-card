<template>
<b-container fluid class="qc-container d-flex justify-content-center align-items-center">
  <b-row class="qc-container__card">
    <b-col cols="12" class="pb-5 pt-5 pl-0 pr-0 text-center qc-container__card__caption">
      <img class="pb-2" :src="logoDark"/>
      <h6>WEB & MEDIA DEVELOPMENT</h6>
      <h6>WWW.QUDOCREATIVE.COM</h6>
    </b-col>
    <b-col class="qc-container__card__contact pb-4 pl-2">
      <Name/>
      <Title/>
      <Phone/>
      <Email/>
    </b-col>
  </b-row>
</b-container>
</template>

<script>

import Name from "@/components/contact-name.vue";
import Title from "@/components/contact-title.vue";
import Phone from "@/components/contact-phone.vue";
import Email from "@/components/contact-email.vue";
import logoDark from "@/assets/logo-dark.png";

export default {
  name: "home",
  components: {
    Name,
    Title,
    Phone,
    Email
  },
  data() {
    return {
      logoDark: logoDark
    }
  }
 
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Abel');
html, body {
  height: 100%;
  width: 100%;
}
  .qc-container {
    background: white;
    min-height: 100vh;
    width: 100vw;
    font-family: 'Abel', sans-serif;

    &__card {
      width: 300px;
      border: solid thick black;

      img {
        width: 95%;
      }

      &__caption {
        h6 {
          font-size: 13px;
          letter-spacing: 5px;
        }
        
      }
    }
  }
</style>
