<template>
    <header>
        <!-- header top -->
        <HeaderTopComponent/>
        <!-- header bottom -->
        <HeaderBottomComponent :navLinks="headerBottomLinks"/>
    </header>
</template>

<script>
// *IMPORTS
import HeaderTopComponent from "./HeaderTopComponent.vue";
import HeaderBottomComponent from "./HeaderBottomComponent.vue";

// *DATA
export default {
    name: "HeaderComponent",
    props: {
        headerBottomLinks: Array,
    },
    components: {
        HeaderTopComponent,
        HeaderBottomComponent,
    },
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>

</style>