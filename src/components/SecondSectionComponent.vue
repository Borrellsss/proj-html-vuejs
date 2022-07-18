<template>
    <section class="light-background">
        <div class="container">
            <span class="before-title small-text">OUR BUSINESS AREAS</span>
            <h2 class="black-title">
                Excellence in
                <span class="word-wrapper word-green">Services</span>
            </h2>
            <div class="second-section-text flex justify-between">
                <p>Lorem ipsum dolor sit amet elit. Eaque rerum sunt eum sit, similique fugiat odio laborum maiores velit vitae distinctio ipsa inventore blanditiis obcaecati molestiae rem.</p>
                <a class="btn green" href="#">SEE ALL</a>
            </div>
            <div class="second-section-cards flex wrap">
                <SecondSectionCardComponent v-for="element in secondSectionCardsArray" :key="element.id" :secondSectionCard="element"/>
            </div>
        </div>
    </section>
</template>

<script>
// *IMPORTS
import SecondSectionCardComponent from "./SecondSectionCardComponent.vue";

export default {
    name: "SecondSectionComponent",
    components: {
        SecondSectionCardComponent,
    },
    props: {

    },
    data() {
        return {
            secondSectionCardsArray: [
                {
                    id: 1,
                    icon: "fa-solid fa-sitemap",
                    title: "Audit & Assurance",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 2,
                    icon: "fa-solid fa-briefcase",
                    title: "Financial Advisory",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 3,
                    icon: "fa-solid fa-chart-simple",
                    title: "Analytics and M&A",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 4,
                    icon: "fa-solid fa-plane",
                    title: "Middle Marketing",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 5,
                    icon: "fa-solid fa-earth-europe",
                    title: "Legal Consulting",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
                },
                {
                    id: 6,
                    icon: "fa-solid fa-box-archive",
                    title: "Regulatory Risk",
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
    background-color: #eef4ed;
}
p {
    width: 73%;
}
.second-section-text {
    margin-bottom: 1rem;
    
    > .btn {
        align-self: flex-start;
    }
} 
.second-section-cards {
    gap: 1.2rem;
}
</style>