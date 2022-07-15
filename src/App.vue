<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent/>
    
    <!-- MAIN -->
    <!-- sections -->

    <!-- FOOTER -->
  </div>
</template>

<script>
// *IMPORTS
import HeaderComponent from "./components/HeaderComponent.vue";

// *DATA
export default {
  name: "App",
  components: {
    HeaderComponent,
  }
}
</script>

<style lang="scss">
// *IMPORTS
@import "./style/common.scss";

</style>
