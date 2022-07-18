<template>
    <section class="dark-background">
        <div class="container small">
            <div class="flex justify-between">
                <div class="sixth-section-left">
                    <span class="before-title small-text">NEWSLETTER</span>
                    <h2 class="white-title">
                        <span class="word-wrapper word-white">Know</span>
                        First
                    </h2>
                    <p>Follow closely and receive content about our company and the news of the current market.</p>
                </div>
                <div class="sixth-section-right">
                    <div class="flex wrap">
                        <input type="text" placeholder="Name">
                        <input type="email" placeholder="Email">
                        <a @click.prevent class="btn green" href="#">SUBSCRIBE</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
// *IMPORTS

export default {
    name: "SixthSectionComponent",
    components: {

    },
    props: {

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
section {
    background: url("../assets/img/bg-1.jpg") center/cover;

    :is(.sixth-section-left, .sixth-section-right) {
        width: 47%;
    }
}
.sixth-section-left > p {
    margin-bottom: 0;
}
.sixth-section-right {
    align-self: flex-end;

    input {
        margin-bottom: 0.85rem;
        width: 100%;
    }
}
</style>