<template>
    <div class="fourth-section-card">
        <div class="flex align-center">
            <div class="member-image">
                <img :src="fourthSectionCard.img" :alt="fourthSectionCard.name">
            </div>
            <div class="member-info">
                <h3 class="member-name">
                    {{fourthSectionCard.name}}
                </h3>
                <span class="member-role">
                    {{fourthSectionCard.role}}
                </span>
                <ul class="member-socials flex">
                    <li v-for="(element, index) in fourthSectionCard.socials" :key="index">
                        <a class="flex justify-center align-center" href="#">
                            <span>
                                <i :class="element"></i>
                            </span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
// *IMPORTS

export default {
    name: "FourthSectionCardComponent",
    components: {

    },
    props: {
        fourthSectionCard: Object,
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
.fourth-section-card {
    width: calc((100% / 2) - 1.05rem);

    > .flex {
        gap: 1.2rem
    }
}
.member-image {
    width: 35%;

    img {
        border-radius: 0.2rem;
    }
}
.member-info {

    .member-name {
        margin-bottom: 0;
    }
    .member-role {
        margin-bottom: 0.8rem;
        display: inline-block;
        font-size: 0.6rem;
    }
    .member-socials {

        li {
            margin-right: 0.2rem;
        }
        a {
            width: 1.6rem;
            aspect-ratio: 1/1;
            font-size: 0.8rem;
            font-weight: 800;
            color: $third-color;
            border-radius: 50%;
            background-color: $word-wrapper-bg-color;

            &:hover {
                box-shadow: 0 0 3px $seventh-color;
            }
        }
    }
}
</style>