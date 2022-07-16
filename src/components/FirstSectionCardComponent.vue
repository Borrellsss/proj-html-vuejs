<template>
    <div class="first-section-card">
        <h3>
            <span class="card-icon">
                <i :class="firstSectionCard.icon"></i>
            </span>
            {{firstSectionCard.title}}
        </h3>
        <p>
            {{firstSectionCard.text}}
        </p>
    </div>
</template>

<script>
// *IMPORTS

export default {
    name: "FirstSectionCardComponent",
    components: {

    },
    props: {
        firstSectionCard: Object,
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
.first-section-card {
    width: calc((100% / 2) - 0.35rem);
}
.card-icon {
    color: $seventh-color;
}
</style>