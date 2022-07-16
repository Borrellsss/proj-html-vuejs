<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent :headerBottomLinks="headerBottomLinks"/>

    <!-- MAIN -->
    <FirstSectionComponent/>
    <SecondSectionComponent/>
    <ThirdSectionComponent/>

    <!-- FOOTER -->
  </div>
</template>

<script>
// *IMPORTS
import HeaderComponent from "./components/HeaderComponent.vue";
import FirstSectionComponent from "./components/FirstSectionComponent.vue";
import SecondSectionComponent from "./components/SecondSectionComponent.vue";
import ThirdSectionComponent from "./components/ThirdSectionComponent.vue";

// *DATA
export default {
  name: "App",
  components: {
    HeaderComponent,
    FirstSectionComponent,
    SecondSectionComponent,
    ThirdSectionComponent,
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
