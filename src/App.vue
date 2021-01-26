<template>
    <div id="app">
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
#app {
    // font-family: Avenir, Helvetica, Arial, sans-serif;
    font-family: 'Fira Sans', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
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
