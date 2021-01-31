<template>
    <div class="aaa">
        <div>2021-01-26</div>

        <header class="header">
            <div class="logo-box">
                <img
                    src="../../assets/images/natours/logo-white.png"
                    alt="image of the logo"
                    class="logo"
                />
            </div>

            <div class="text-box">
                <h1 class="heading-primary">
                    <span class="heading-primary-main">Outdoors</span>
                    <span class="heading-primary-sub"
                        >is where life happens</span
                    >
                </h1>
                <a href="" class="btn btn-white btn-sliding"> Discover our tours </a>
            </div>
        </header>
    </div>
</template>

<style lang="scss" scoped>
// Light green: #7ed56f
// Medium green: #55c57a
// Dark green: #28b485

// resetting
* {
    box-sizing: border-box;
    font-size: 1em;
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
    position: relative;
    clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
}

.logo-box {
    left: 40px;
    position: absolute;
    top: 40px;
}

.logo {
    height: 35px;
}

.heading-primary {
    align-items: center;
    backface-visibility: hidden; // fix the jolt at animation end
    // background-color: red;
    color: #fff;
    display: flex;
    flex-direction: column;
    margin-bottom: 3em;
    text-transform: uppercase;

    &-main {
        // display: block;
        // animation-delay: 3s;
        animation-duration: 1s;
        animation-name: slideInFromLeft;
        animation-timing-function: ease-out;
        font-size: 60px;
        font-weight: 400px;
        letter-spacing: 35px;
    }
    &-sub {
        // display: block;
        animation: slideInFromRight 1s ease-out;
        font-size: 20px;
        font-weight: 700;
        letter-spacing: 17.4px;
    }
}

.text-box {
    left: 50%;
    position: absolute;
    top: 40%;
    transform: translate(-50%, -50%);
}

@keyframes slideInFromLeft {
    // start
    0% {
        opacity: 0;
        transform: translateX(-100px); // on the abscissa
    }
    80% {
        transform: translateX(10px);
    }
    // finish
    100% {
        opacity: 1;
        transform: translateX(0px); // on the abscissa
    }
}

@keyframes slideInFromRight {
    // start
    0% {
        opacity: 0;
        transform: translateX(100px); // on the abscissa
    }
    80% {
        transform: translateX(-10px);
    }
    // finish
    100% {
        opacity: 1;
        transform: translateX(0px); // on the abscissa
    }
}

.btn {
    position: relative;
    &:active {
        box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
        transform: translateY(-1px); // move 1 px up
    }
    &::after {
        border-radius: 100px;
        content: "";
        display: inline-block;
        height: 100%;
        left: 0;
        position: absolute;
        top: 0;
        transition: all 0.4s;
        width: 100%;
        z-index: -1;
    }
    &:hover {
        box-shadow: 0 10px 10px rgba(0, 0, 0, 0.2);
        transform: translateY(-3px); // move 3 px up

        &::after {
            opacity: 0;
            transform: scaleX(1.5) scaleY(1.6);
        }
    }
    &:link,
    &:visited {
        border-radius: 100px;
        display: inline-block;
        padding: 15px 40px;
        text-decoration: none;
        text-transform: uppercase;
        transition: all 0.2s;
    }
    &-white {
        background-color: #fff;
        color: #777;
        &::after {
            background-color: #fff;
        }
    }
    &-sliding {
        animation: slideInFromBottom .5s ease-out .75s;
        animation-fill-mode: backwards;
    }
}
@keyframes slideInFromBottom {
    // start
    0% {
        opacity: 0;
        transform: translateY(30px); // on the ordinate
    }
    // finish
    100% {
        opacity: 1;
        transform: translateY(0px); // on the ordinate
    }
}
</style>

