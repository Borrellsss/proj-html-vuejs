<template>
    <section class="light-background">
        <div class="container">
            <span class="before-title small-text">OUR EDITORIAL CONTENT</span>
            <h2 class="black-title">
                Latest
                <span class="word-wrapper word-green">News</span>
            </h2>
            <div class="fifth-section-text flex justify-between">
                <p>Every week we publish content about what is best in the business world.</p>
                <a @click.prevent class="btn green" href="#">SEE ALL</a>
            </div>
            <div class="fifth-section-cards flex wrap">
                <FifthSectionCardComponent v-for="element in fifthSectionCardsArray" :key="element.id" :fifthSectionCard="element"/>
            </div>
        </div>
    </section>
</template>

<script>
// *IMPORTS
import FifthSectionCardComponent from "./FifthSectionCardComponent.vue";

export default {
    name: "FifthSectionComponent",
    components: {
        FifthSectionCardComponent,
    },
    props: {

    },
    data() {
        return {
            fifthSectionCardsArray: [
                {
                    id: 1,
                    img: require("../assets/img/news-1.jpg"),
                    text: "Increasing creativity is possible for everyone",
                },
                {
                    id: 2,
                    img: require("../assets/img/news-2.jpg"),
                    text: "Because market research is part of the business plan",
                },
                {
                    id: 3,
                    img: require("../assets/img/news-3.jpg"),
                    text: "Working from home is now a trend",
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
    background-color: $second-color;

    h2 {
        margin-bottom: 0rem;
    }
}
.fifth-section-text {
    margin-bottom: 2rem;

    p {
        margin-bottom: 0;
        width: 73%;
        align-self: flex-end;
    }
} 
.fifth-section-cards {
    gap: 1.2rem;
}
</style>