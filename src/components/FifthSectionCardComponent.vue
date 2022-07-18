<template>
    <div class="fifth-section-card">
        <div class="card-image">
            <img :src="fifthSectionCard.img" alt="">
        </div>
        <h3 class="card-text">
            {{fifthSectionCard.text}}
        </h3>
    </div>
</template>

<script>
// *IMPORTS

export default {
    name: "FifthSectionCardComponent",
    components: {

    },
    props: {
        fifthSectionCard: Object,
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
.fifth-section-card {
    width: calc((100% / 3) - 0.8rem);
    position: relative;

    > .card-text {
        padding: 1.2rem;
        position: absolute;
        left: 0;
        bottom: 0;
        text-align: center;
        color: $second-color;
    }
}
.card-image {
    border-radius: 0.45rem;
    overflow: hidden;

    > img {
        filter: brightness(55%) grayscale(10%);
        transition: transform 800ms;

        &:hover {
            transform: scale(1.08);
        }
    }
}
</style>