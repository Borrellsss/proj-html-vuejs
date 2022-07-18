<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent :headerBottomLinks="headerBottomLinks"/>

    <!-- MAIN -->
    <main>
      <FirstSectionComponent/>
      <SecondSectionComponent/>
      <ThirdSectionComponent/>
      <FourthSectionComponent/>
      <FifthSectionComponent/>
      <SixthSectionComponent/>
    </main>

    <!-- FOOTER -->
    <FooterComponent :footerLinks="footerTopLinks"/>
  </div>
</template>

<script>
// *IMPORTS
import HeaderComponent from "./components/HeaderComponent.vue";
import FirstSectionComponent from "./components/FirstSectionComponent.vue";
import SecondSectionComponent from "./components/SecondSectionComponent.vue";
import ThirdSectionComponent from "./components/ThirdSectionComponent.vue";
import FourthSectionComponent from "./components/FourthSectionComponent.vue";
import FifthSectionComponent from "./components/FifthSectionComponent.vue";
import SixthSectionComponent from "./components/SixthSectionComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

// *DATA
export default {
  name: "App",
  components: {
    HeaderComponent,
    FirstSectionComponent,
    SecondSectionComponent,
    ThirdSectionComponent,
    FourthSectionComponent,
    FifthSectionComponent,
    SixthSectionComponent,
    FooterComponent,
  },
  data() {
    return {
      headerBottomLinks: ["home", "about", "services", "process", "team", "blog"],
      footerTopLinks: [
        {
          id: 1,
          title: "About",
          links: ["The Company", "Institutional", "Social & Events", "Innovation", "Environment", "Technology"],
        },
        {
          id: 2,
          title: "Services",
          links: ["Audit & Assurance", "Financial Advisory", "Analytics M&A", "Middle Marketing", "Legal Consulting", "Regulatory Risk"],
        },
        {
          id: 3,
          title: "Support",
          links: ["Responsibility", "Terms of Use", "About Cookies", "Privacy Policy", "Accessibility", "Information"],
        },
      ]
    }
  }
}
</script>

<style lang="scss">
// *IMPORTS
@import "./style/common.scss";

</style>
