<template>
    <div class="home">
        <div class="photo">
            <div class="photo-image"></div>
        </div>
        <Intro msg="Hi" />
    </div>
</template>

<script>
// @ is an alias to /src
import Intro from "@/components/Intro.vue";

export default {
    name: "Home",
    components: {
        Intro,
    },
};
</script>

<style lang="scss">
$img-size: 10em;
.photo {
    display: flex;
    justify-content: center;
    .photo-image {
        background-image: url("../assets/me.jpg");
        background-repeat: no-repeat;
        background-size: $img-size;
        border-radius: 50%;
        height: $img-size;
        width: $img-size;
    }
}
</style>
