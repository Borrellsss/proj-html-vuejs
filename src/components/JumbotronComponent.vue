<template>
    <div class="jumbotron flex align-center">
        <div class="fusions">
            <span class="before-title">FUSIONS & ACQUISITIONS</span>
            <h1>Insurance Consulting</h1>
            <div class="jumbotron-inputs flex wrap">
                <input type="text" placeholder="Name">
                <input type="email" placeholder="Email">
                <input type="text" placeholder="Phone">
                <select name="" id="">
                    <option value="more">More Info</option>
                </select>
            </div>
            <div class="jumbotron-buttons">
                <a class="btn green" href="#">GET IN TOUCH</a>
                <a class="btn transparent" href="#">READ MORE</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "JumbotronComponent",
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/variables.scss";

// *STYLING
.jumbotron {
    height: 535px;
}
.fusions {
    margin-left: auto;
    width: 45%;
}
.jumbotron-inputs {
    margin-top: 1rem;
    gap: 0.7rem;

    :is(input, select) {
        width: calc((100% / 2) - 0.35rem);
        background-color: #aeb0b060;
    }
}
.jumbotron-buttons {
    margin-top: 0.7rem;

    a {
        margin-right: 0.7rem;
    }
}
</style>