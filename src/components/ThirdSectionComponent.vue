<template>
    <section class="light-background">
        <div class="third-section-top">
            <div class="container">
                <span class="before-title small-text">HOW IT WORKS IN PRACTICE</span>
                <h2>
                    <span class="word-wrapper word-green">Process</span>
                    Management
                </h2>
                <p class="third-section-top-text">We work with innovative methodologies to ensure that the entire reformatting process is done from start to finish as planned.</p>
            </div>
        </div>
        <div class="third-section-bottom">
            <div class="container big">
                <ul class="flex">
                    <ThirdSectionCardComponent v-for="element in thirdSectionCardsArray" :key="element.id" :thirdSectionCard="element"/>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
// *IMPORTS
import ThirdSectionCardComponent from "./ThirdSectionCardComponent.vue";

export default {
    name: "ThirdSectionComponent",
    components: {
        ThirdSectionCardComponent,
    },
    props: {

    },
    data() {
        return {
            thirdSectionCardsArray: [
                {
                    id: 1,
                    title: "Collection of information",
                    text: "Lorem ipsum dolor sit amet consecteur.",
                },
                {
                    id: 2,
                    title: "Strategic planning",
                    text: "Lorem ipsum dolor sit amet consecteur.",
                },
                {
                    id: 3,
                    title: "Assignment of responsibilities",
                    text: "Lorem ipsum dolor sit amet consecteur.",
                },
                {
                    id: 4,
                    title: "Formatting process",
                    text: "Lorem ipsum dolor sit amet consecteur.",
                },
                {
                    id: 5,
                    title: "Continuity formalization",
                    text: "Lorem ipsum dolor sit amet consecteur.",
                },
            ]
        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/variables.scss";

// *STYLING
section {
    padding-block: $main-sections-padding calc($main-sections-padding - 1.1rem);
}
.third-section-top {
    padding-bottom: 3.5rem;
    border-bottom: 3.5px solid #daeced;
    text-align: center;

    .third-section-top-text {
        margin: 0 auto;
        width: 67%;
    }
}
.third-section-bottom {
    position: relative;
    top: -1.1rem;
    z-index: 99;

    .flex {
        gap: 1.5rem;
    }
}
</style>