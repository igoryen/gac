<template>
    <div class="home">
        <div class="photo">
            <div class="photo-image"></div>
        </div>
        <Intro msg="Hi!" />
        <proj-list />
    </div>
</template>

<script>
// @ is an alias to /src
import Intro from "@/components/Intro.vue";
import ProjList from "@/components/ProjList";

export default {
    name: "Home",
    components: {
        Intro,
        ProjList,
    },
};
</script>

<style lang="scss">
.html {
    font-family: "Fira Sans", sans-serif;
}
$img-size: 10em;
.photo {
    display: flex;
    justify-content: center;
    .photo-image {
        background-image: url("../assets/me-a.jpg");
        background-repeat: no-repeat;
        background-size: $img-size;
        border-radius: 50%;
        height: $img-size;
        width: $img-size;
    }
}
</style>
