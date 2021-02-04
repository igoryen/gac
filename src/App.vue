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
    font-size: 62.5%; // DR%
    // DR% (the Design's Root font-size in percentage that must be typed in CSS)
    // DRpx (the Design's Root font-size the design is based on, in pixels (e.g. 10px))
    // Bpx (the Browser's font-size setting in pixels 
    //     (the default is 16px, but can be customized by user)
    // Calculation:
    // DR% = RRpx/Bpx = 10px/16px = 0.625 = 62.5%
    // if Bpx = 16px, then DRpx = DR% of Bpx = 62.5% of 16px = 10px
    // if Bpx = 20px, then DRpx = DR% of Bpx = 62.5% of 20px = 12.5px
    // if Bpx = 22px, then DRpx = DR% of Bpx = 62.5% of 22px = 13.75px
}

body {
    box-sizing: border-box;
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
