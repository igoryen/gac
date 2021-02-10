<template>
    <div id="app" class="app">
        <Slide :closeOnNavigation="true">
            <div id="nav">
                <router-link to="/">Home</router-link>
                <router-link to="/about">About</router-link>
                <router-link to="/css-projects">CSS Projects</router-link>
            </div>
        </Slide>

        <router-view />
    </div>
</template>

<script>
import { Slide } from "vue-burger-menu";
export default {
    components: {
        Slide,
    },
};
</script>

<style lang="scss">
@import "../src/assets/scss/main.scss";

#nav {
    align-items: flex-start;
    display: flex;
    flex-direction: column;
    a {
        // color: #2c3e50;
        color: $color-white;
        font-weight: bold;
        margin-bottom: 1em;
        &.router-link-exact-active {
            color: color-green;
        }
    }
}

// #nav a.router-link-exact-active {
//     color: #42b983;
// }
</style>
