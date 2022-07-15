<template>
    <div class="header-bottom">
        <div class="container">
            <div class="flex justify-between align-center">
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
        </div>
        <!-- <div v-for="element, index in navLinks" :key="index">{{element.toUpperCase()}}</div> -->
    </div>
</template>

<script>
// *IMPORTS

// *DATA
export default {
    name: "HeaderBottomComponent",
    props: {
        navLinks: Array,
    }
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/variables.scss";

// *STYLING
.header-bottom {
    padding-block: $header-padding;
    font-size: 0.7rem;
    color: $twentieth-color;
    background-color: $eleventh-color;
}
.header-bottom-right li {
    margin-left: 1.5rem;
}
</style>