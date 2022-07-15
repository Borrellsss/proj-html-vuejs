<template>
    <header>
        <!-- header top -->
        <HeaderTopComponent/>
        <!-- header bottom -->
        <HeaderBottomComponent/>
    </header>
</template>

<script>
// *IMPORTS
import HeaderTopComponent from "./HeaderTopComponent.vue";
import HeaderBottomComponent from "./HeaderBottomComponent.vue";

// *DATA
export default {
    name: "HeaderComponent",
    components: {
        HeaderTopComponent,
        HeaderBottomComponent,
    }
}
</script>

<style lang="scss" scoped>

</style>