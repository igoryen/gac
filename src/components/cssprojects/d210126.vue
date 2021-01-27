<template>
    <div class="aaa">
        <div>2021-01-26</div>

        <header class="header">Some text...</header>
    </div>
</template>

<style lang="scss" scoped>
// Light green: #7ed56f
// Medium green: #55c57a
// Dark green: #28b485

// resetting
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

.aaa {
    color: #777;
    font-family: "Lato", sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 1.7;
}

.header {
    height: 95vh;
    background-image: linear-gradient(
            to right bottom,
            rgba(126, 213, 111, 0.8),
            rgba(40, 180, 133, 0.8)
        ),
        url(../../assets/images/natours/hero.jpg);
    background-size: cover;
    background-position: top;
    clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
}
</style>

