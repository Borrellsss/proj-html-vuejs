<template>
    <section class="dark-background">
        <div class="container">
            <div class="flex justify-between">
                <div class="fourth-section-left">
                    <div class="fourth-section-left-top">
                        <span class="before-title small-text">WE LIKE WHAT WE DO</span>
                        <h2>
                            <span class="word-wrapper word-white">Team</span>
                            of Experts
                        </h2>
                        <p>
                            Ethics and integrity are the bases on which our professionals build their careers.<br>
                            They are foundamentals that become daily attitudes.
                        </p>
                    </div>
                    <div class="fourth-section-left-bottom flex wrap">
                        <FourthSectionCardComponent v-for="element in fourthSectionCardsArray" :key="element.id" :fourthSectionCard="element"/>
                    </div>
                </div>
                <div class="fourth-section-right">
                    <h3>President Speech</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing consectetur elit. Aut quis, ad cupiditate.</p>
                    <p>Lorem ipsum dolor sit amet consectetur elit. Eveniet vel atque minus odio autem nisi nam, aliquam omnis vero ut architecto unde, velit odit id nemo quisquam.</p>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint dignissimos fuga expedita magni.</p>
                    <div class="flex justify-between align-center">
                        <h4>T. Johnson</h4>
                        <span class="quotation-marks-icon">
                            <i class="fa-solid fa-quote-right"></i>
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
// *IMPORTS
import FourthSectionCardComponent from "./FourthSectionCardComponent.vue";

export default {
    name: "FourthSectionComponent",
    components: {
        FourthSectionCardComponent,
    },
    props: {

    },
    data() {
        return {
            fourthSectionCardsArray: [
                {
                    id: 1,
                    img: require("../assets/img/team-1.jpg"),
                    name: "David Cooper",
                    role: "CTO & CO-FOUNDER",
                    socials: ["fa-brands fa-facebook-f", "fa-brands fa-twitter", "fa-brands fa-linkedin-in"],
                },
                {
                    id: 2,
                    img: require("../assets/img/team-3.jpg"),
                    name: "Oliver Jones",
                    role: "CHIEF PROCUREMENT",
                    socials: ["fa-brands fa-facebook-f", "fa-brands fa-twitter", "fa-brands fa-linkedin-in"],
                },
                {
                    id: 3,
                    img: require("../assets/img/team-2.jpg"),
                    name: "Emma Lopez",
                    role: "CHIEF MARKETING",
                    socials: ["fa-brands fa-facebook-f", "fa-brands fa-twitter", "fa-brands fa-linkedin-in"],
                },
                {
                    id: 4,
                    img: require("../assets/img/team-4.jpg"),
                    name: "T. Johnson",
                    role: "CEO & PRESIDENT",
                    socials: ["fa-brands fa-facebook-f", "fa-brands fa-twitter", "fa-brands fa-linkedin-in"],
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
}
.fourth-section-left {
    width: 60%;

    .fourth-section-left-top > p {
        margin-bottom: 2.2rem;
    }
}
.fourth-section-left-bottom {
    gap: 2.1rem;
}
.fourth-section-right {
    padding: 1.5rem;
    width: 32%;
    border-radius: 0.2rem;
    align-self: flex-end;
    background-color: $seventeenth-color;

    h3 {
        font-weight: 900;
    }
    h4 {
        margin-bottom: 0;
    }
    p {
        font-weight: 300;
    }
}
.quotation-marks-icon {
    font-size: 1.3rem;
    color: #046162;
}
</style>