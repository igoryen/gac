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

.home {
    color: #777;
    font-family: "Lato", sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 1.7;

    text-align: center;
    color: #2c3e50;
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
