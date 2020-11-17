<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
        <h2>igoryen here.</h2>
        <p>
            Feel free to
            <a
                class="download-stuff"
                href="/cv/Igor_Entaltsev_Frontend_Dev_and_UX_UI_Design_v24.pdf"
                target="_blank"
                >download &#x1F4E5; my resume</a
            >
            and check out my frontend projects below.
        </p>
        <p></p>
    </div>
</template>

<script>
export default {
    name: "Intro",
    props: {
        msg: String,
    },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.hello {
    margin-bottom: 3em;
    p {
        line-height: 2;
        margin: 0 1em;
    }
}

.download-stuff {
    background-color: lighten(purple, 72%);
    padding: 0.2em 0.5em;
    border-radius: 10px;
    text-decoration: none;
    transition: all 0.3s;
    &:hover {
        background-color: darken(purple, 10%);
    }
}

h3 {
    margin: 40px 0 0;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: inline-block;
    margin: 0 10px;
}
a {
    color: #42b983;
}
</style>
