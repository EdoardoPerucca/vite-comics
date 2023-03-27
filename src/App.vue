<script>

import HeaderSection from "./components/HeaderSection.vue";
import ContentSection from "./components/ContentSection.vue";
import ShopSection from "./components/ShopSection.vue";
import MainSection from "./components/MainSection.vue";
import FooterSection from "./components/FooterSection.vue";
import '@fortawesome/fontawesome-free/css/all.css';

export default {
  data() {
    return {

    }
  },

  components: {
    HeaderSection,
    ContentSection,
    ShopSection,
    MainSection,
    FooterSection,
  },

}
</script>

<template>
  <div id="vue-container">
    <HeaderSection></HeaderSection>

    <ContentSection></ContentSection>

    <ShopSection></ShopSection>

    <MainSection id="main"></MainSection>

    <FooterSection id="footer"></FooterSection>

  </div>
</template>

<style scoped lang="scss">
#vue-container {
  width: 100vw;
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;


}
</style>