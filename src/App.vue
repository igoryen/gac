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

html {
    font-size: 10px;
}

body {
    color: #777;
    font-family: "Lato", sans-serif;
    // font-size: 16px;
    font-weight: 400;
    line-height: 1.7;
}

#nav {
    align-items: flex-start;
    display: flex;
    flex-direction: column;
    a {
        // color: #2c3e50;
        color: gray;
        font-weight: bold;
        margin-bottom: 1em;
        &.router-link-exact-active {
            color: #42b983;
        }
    }
}

// #nav a.router-link-exact-active {
//     color: #42b983;
// }
</style>
