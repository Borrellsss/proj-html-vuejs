<template>
    <li class="third-section-card">
        <span class="card-number flex justify-center align-center">
            0{{thirdSectionCard.id}}
        </span>
        <h3>
            {{thirdSectionCard.title}}
        </h3>
        <p>
            {{thirdSectionCard.text}}
        </p>
    </li>
</template>

<script>
// *IMPORTS

export default {
    name: "ThirdSectionCardComponent",
    components: {

    },
    props: {
        thirdSectionCard: Object,
    },
    data() {
        return {

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
.third-section-card {
    width: calc((100% / 5) - 1.2rem);
    text-align: center;
}
.card-number {
    margin: 0 auto 0.9rem;
    width: 1.9rem;
    aspect-ratio: 1/1;
    font-size: 0.8rem;
    font-weight: 700;
    color: $third-color;
    border-radius: 50%;
    background-color: #daeced;
}
</style>