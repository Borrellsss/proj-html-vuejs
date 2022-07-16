<template>
    <div class="header-bottom">
        <div class="container">
            <div class="header-bottom-top flex justify-between align-center">
                <div class="header-bottom-left">
                    LOGO (MISSING!!!)
                </div>
                <nav class="header-bottom-right">
                    <ul class="flex align-center">
                        <li v-for="element, index in navLinks" :key="index">
                            <a href="#">
                                {{element.toUpperCase()}}
                            </a>
                        </li>
                        <li>
                            <a class="btn green" href="#">GET IN TOUCH</a>
                        </li>
                    </ul>
                </nav>
            </div>
            <JumbotronComponent/>
        </div>
        <!-- <div v-for="element, index in navLinks" :key="index">{{element.toUpperCase()}}</div> -->
    </div>
</template>

<script>
// *IMPORTS
import JumbotronComponent from "./JumbotronComponent.vue";

// *DATA
export default {
    name: "HeaderBottomComponent",
    props: {
        navLinks: Array,
    },
    components: {
        JumbotronComponent,
    },
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/variables.scss";

// *STYLING
.header-bottom {
    font-size: 0.7rem;
    color: $twentieth-color;
    background: url("../assets/img/bg-6.jpg") center/cover;
}
.header-bottom-top {
    padding-block: $header-padding 0;
}
.header-bottom-right li {
    margin-left: 1.5rem;
}
</style>