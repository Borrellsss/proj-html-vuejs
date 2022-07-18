<template>
    <div class="second-section-card">
        <div class="flex justify-between">
            <span class="card-icon">
                <i :class="secondSectionCard.icon"></i>
            </span>
            <span class="arrow">
                <a href="#">
                    <i class="fa-solid fa-arrow-right"></i>
                </a>
            </span>
        </div>
        <h3>
            {{secondSectionCard.title}}
        </h3>
        <p>
            {{secondSectionCard.text}}
        </p>
    </div>
</template>

<script>
// *IMPORTS

export default {
    name: "SecondSectionCardComponent",
    components: {

    },
    props: {
        secondSectionCard: Object,
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
.second-section-card {
    padding: 2rem;
    width: calc((100% / 3) - 0.8rem);
    background-color: $second-color;
    border-radius: 0.4rem;

    .flex {
        margin-bottom: 0.75rem;
    }
}
.card-icon {
    font-size: 1.8rem;
    color: $third-color;
}
.arrow {
    color: $seventh-color;
    transition: transform 200ms;

    &:hover {
        transform: scale(1.1);
    }
}
.fa-solid.fa-plane {
    transform: rotatez(-45deg);
}
</style>