<template>
    <section class="dark-background">
        <div class="container">
            <div class="flex justify-between">
                <div class="first-section-left">
                    <span class="before-title small-text">ABOUT THE NETWORK</span>
                    <h2 class="white-title">
                        <span class="word-wrapper word-white">The</span>
                        Company
                    </h2>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sit vitae corrupti odit blanditiis aut numquam eligendi quia at est sequi rerum eaque ut harum, itaque tenetur id vero natus dolor.</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi ratione ad rerum eius nam quasi nisi.</p>
                </div>
                <div class="first-section-right">
                    <div class="first-section-cards flex wrap">
                        <FirstSectionCardComponent v-for="element in firstSectionCardsArray" :key="element.id" :firstSectionCard="element"/>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
// *IMPORTS
import FirstSectionCardComponent from "./FirstSectionCardComponent.vue"

export default {
    name: "FirstSectionComponent",
    components: {
        FirstSectionCardComponent,
    },
    props: {

    },
    data() {
        return {
            firstSectionCardsArray: [
                {
                    id: 1,
                    icon: "fa-solid fa-award",
                    title: "Tradition",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 2,
                    icon: "fa-solid fa-lock",
                    title: "Security",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 3,
                    icon: "fa-solid fa-pen-to-square",
                    title: "Certificate",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 4,
                    icon: "fa-solid fa-graduation-cap",
                    title: "Expertise",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
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
    background-color: $first-color;

    :is(.first-section-left, .first-section-right) {
        width: 46%;
    }
}
.first-section-right {
    align-self: flex-end;

    > .first-section-cards {
        gap: 0.7rem;
    }
}
</style>