<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent :headerBottomLinks="headerBottomLinks"/>

    <!-- MAIN -->
    <FirstSectionComponent/>
    <SecondSectionComponent/>
    <ThirdSectionComponent/>
    <FourthSectionComponent/>
    <FifthSectionComponent/>

    <!-- FOOTER -->
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
  },
  data() {
    return {
      headerBottomLinks: ["home", "about", "services", "process", "team", "blog"],
    }
  }
}
</script>

<style lang="scss">
// *IMPORTS
@import "./style/common.scss";

</style>
