<template>
    <div class="header-top">
        <div class="container">
            <div class="flex justify-between">
                <div class="header-top-left">
                    <span>
                        <span>
                            <i class="fa-solid fa-clock"></i>
                        </span>
                        Open Hours: Mon - Sat - 9:00 - 18:00
                    </span>
                </div>
                <div class="header-top-right">
                    <ul class="contacts flex">
                        <li>
                            <a href="#">
                                <span>
                                    <i class="fa-solid fa-phone"></i>
                                </span>
                                +1 (305) 1234-5678
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <span>
                                    <i class="fa-solid fa-envelope"></i>
                                </span>
                                hello@example.com
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <span>
                                    <i class="fa-brands fa-facebook-f"></i>
                                </span>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <span>
                                    <i class="fa-brands fa-twitter"></i>
                                </span>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <span>
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </span>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
// *IMPORTS

// *DATA
export default {
    name: "HeaderTopComponent",
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/variables.scss";

// *STYLING
.header-top {
    padding-block: $header-padding;
    font-size: $header-top-font-size;
    color: #c0c3d0;
    background-color: $twentieth-color;
}
.contacts > li {
    margin-left: 1.5rem;
}
.fa-clock,
.fa-phone,
.fa-envelope {
    margin-right: 0.15rem;
}
</style>