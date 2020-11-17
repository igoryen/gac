<template>
    <a class="proj-list-card" :href="item.link" target="_blank">
        <div
            class="bkgimg"
            :style="
                'background-image: url(' +
                require('@/assets/projects/' + item.image) +
                ')'
            "
        ></div>
        <div class="info">
            <h2>
                <span>{{ item.title }}</span>
            </h2>
            <div>
                <span>{{ item.desc }}</span>
            </div>
            <div v-if="item.for">
                <span>For: {{ item.for }}</span>
            </div>
            <div>
                <span>{{ item.date }}</span>
            </div>
        </div>
    </a>
</template>

<script>
export default {
    name: "ProjListItem",
    props: ["item"],
};
</script>

<style lang="scss">
.proj-list-card {
    border-radius: 3px;
    box-shadow: 1px 1px 3px 1px #757474;
    color: #0c0909;
    overflow: hidden;
    position: relative;
    text-decoration: none;
    transition: all 0.3s;

    .bkgimg {
        background-size: cover;
        background-position: center;
        filter: blur(2px);
        transition: all 0.3s;
        height: 100%;
        z-index: -1;
        overflow: hidden;
    }
    .info {
        display: flex;
        flex-direction: column;
        justify-content: center;
        left: 0;
        margin-top: 1em;
        position: absolute;
        top: 0;

        width: 100%;
        h2 {
            margin: 0;
        }
        span {
            background-color: #ffffff;
            border: 1px solid #bebbbb;
            border-radius: 5px;
            line-height: 1.7;
            margin: 1px;
            padding: 3px;
            transition: all 0.3s;
        }
    }

    &:hover {
        .bkgimg {
            filter: blur(0px);
            transform: scale(1.05) rotate(1deg);
            z-index: -1;
        }
        .info {
            span {
                background-color: transparent;

                border: 1px solid transparent;

                text-shadow: #ffffff 1px 0 2px;
            }
        }
    }
    img {
        width: 10em;
    }
}
</style>