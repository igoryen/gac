<template>
    <div class="aaa">
        <div>2021-01-26</div>

        <header class="header">
            <div class="header__logo-box">
                <img
                    src="../../assets/images/natours/logo-white.png"
                    alt="image of the logo"
                    class="header__logo"
                />
            </div>

            <div class="header__text-box">
                <h1 class="heading-primary">
                    <span class="heading-primary--main">Outdoors</span>
                    <span class="heading-primary--sub"
                        >is where life happens</span
                    >
                </h1>
                <a href="" class="btn btn--white btn--sliding">
                    Discover our tours
                </a>
            </div>
        </header>
    </div>
</template>

<style lang="scss" scoped>
@import "../../assets/scss/main.scss";
// resetting
*,
*::after,
*::before {
    box-sizing: inherit;
    font-size: 1em;
    margin: 0;
    padding: 0;
}

.aaa {
    padding-top: 5rem;
}

.header {
    height: 95vh;
    background-image: linear-gradient(
            to right bottom,
            rgba($color-primary-light, 0.8),
            rgba($color-primary-dark, 0.8)
        ),
        url(../../assets/images/natours/hero.jpg);
    background-size: cover;
    background-position: top;
    position: relative;
    clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);

    &__logo {
        height: 3.5rem;

        &-box {
            left: 4rem;
            position: absolute;
            top: 4rem;
        }
    }

    &__text-box {
        left: 50%;
        position: absolute;
        top: 40%;
        text-align: center;
        transform: translate(-50%, -50%);
    }
}

.heading-primary {
    align-items: baseline;
    backface-visibility: hidden; // fix the jolt at animation end
    // background-color: red;
    color: $color-white;
    display: flex;
    flex-direction: column;
    margin-bottom: 6rem;
    text-transform: uppercase;

    &--main {
        // display: block;
        // animation-delay: 3s;
        animation-duration: 1s;
        animation-name: slideInFromLeft;
        animation-timing-function: ease-out;
        font-size: 6rem;
        font-weight: 400px;
        letter-spacing: 3.5rem;
    }
    &--sub {
        // display: block;
        animation: slideInFromRight 1s ease-out;
        font-size: 2rem;
        font-weight: 700;
        letter-spacing: 1.75rem;
    }
}

@keyframes slideInFromLeft {
    // start
    0% {
        opacity: 0;
        transform: translateX(-10rem); // on the abscissa
    }
    80% {
        transform: translateX(1rem);
    }
    // finish
    100% {
        opacity: 1;
        transform: translateX(0); // on the abscissa
    }
}

@keyframes slideInFromRight {
    // start
    0% {
        opacity: 0;
        transform: translateX(10rem); // on the abscissa
    }
    80% {
        transform: translateX(-1rem);
    }
    // finish
    100% {
        opacity: 1;
        transform: translateX(0px); // on the abscissa
    }
}

.btn {
    font-size: 1.6rem;
    position: relative;

    &:active {
        box-shadow: 0 0.5rem 2rem rgba($color-black, 0.2);
        transform: translateY(-0.1rem); // move 1 px up
    }
    &::after {
        border-radius: 10rem;
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
        box-shadow: 0 1rem 1rem rgba($color-black, 0.2);
        transform: translateY(-0.3rem); // move 3 px up

        &::after {
            opacity: 0;
            transform: scaleX(1.5) scaleY(1.6);
        }
    }
    &:link,
    &:visited {
        border-radius: 10rem;
        display: inline-block;
        padding: 1.5rem 4rem;
        text-decoration: none;
        text-transform: uppercase;
        transition: all 0.2s;
    }
    &--white {
        background-color: $color-white;
        color: $color-grey-dark;
        
        &::after {
            background-color: $color-white;
        }
    }
    &--sliding {
        animation: slideInFromBottom 0.5s ease-out 0.75s;
        animation-fill-mode: backwards;
    }
}
@keyframes slideInFromBottom {
    // start
    0% {
        opacity: 0;
        transform: translateY(3rem); // on the ordinate
    }
    // finish
    100% {
        opacity: 1;
        transform: translateY(0); // on the ordinate
    }
}
</style>

