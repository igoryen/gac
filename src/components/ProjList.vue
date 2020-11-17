<template>
    <div>
        <h2>My projects</h2>
        <div class="proj-list-container">
            <ProjListItem
                v-bind:item="item"
                v-for="item in items"
                v-bind:key="item.id"
            />
        </div>
    </div>
</template>

<script>
import ProjListItem from "./ProjListItem";
export default {
    name: "ProjList",
    components: { ProjListItem },
    data() {
        return {
            items: [
                {
                    id: 8,
                    title: "Emblica",
                    desc: "a React app to learn English",
                    link: "https://emblica.herokuapp.com/",
                    date: "2020",
                    image: "emblica.png",
                    for: "my wife",
                },
                {
                    id: 7,
                    title: "Dragonfruit",
                    desc: "a React app to learn Spanish verbs",
                    link: "https://dragonfruit.herokuapp.com/",
                    date: "2020",
                    image: "dragonfruit.png",
                    for: "myself",
                },
                {
                    id: 6,
                    title: "Expensify",
                    desc: "a React app to learn React",
                    link: "https://igoryen-expensify.herokuapp.com/",
                    date: "2020",
                    image: "expensify.png",
                    for: "myself",
                },
                {
                    id: 5,
                    title: "NAS Mobile App",
                    desc: "UI by me",
                    link:
                        "https://apps.apple.com/ca/app/valuation-mobile-app/id536228581#?platform=iphone",
                    date: "2019",
                    image: "nas.png",
                    for: "the Nationwide Group",
                },
                {
                    id: 4,
                    title: "CNX",
                    desc: "WordPress brochure website",
                    link: "https://www.connexionssoftware.com/",
                    date: "2019",
                    image: "cnx.png",
                    for: "the Nationwide Group",
                },
                {
                    id: 3,
                    title: "NRS",
                    desc: "WordPress brochure site, bilingual",
                    link: "https://www.nwrs.ca/",
                    date: "2018",
                    image: "nrs.png",
                    for: "the Nationwide Group",
                },
                {
                    id: 2,
                    title: "HCS",
                    link: "http://nwhcs.ca/How_it_Works.html",
                    desc: "Static website, improved by me (WIP)",
                    date: "2018",
                    image: "hcs.png",
                    for: "the Nationwide Group",
                },
                {
                    id: 1,
                    title: "Lexus.ca",
                    desc: "Multiple pages, design implementation",
                    link: "https://www.lexus.ca/lexus/en",
                    date: "2015-2016",
                    image: "lexus.png",
                    for: "Saatchi & Saatchi",
                },

                {
                    id: 9,
                    title: "Github",
                    desc: "My github account",
                    link: "https://github.com/igoryen",
                    date: "since 2013",
                    image: "github.png",
                },
                // {
                //     id: ,
                //     title: "",
                //     desc: "",
                //     link: "",
                //     date: "",
                // },
            ],
        };
    },
    methods: {},
};
</script>
<style lang="scss">
@media only screen and (min-width: 220px) {
    .proj-list-container {
        display: grid;
        grid-gap: 2em;
        grid-template-columns: minmax(220px, 300px);
        grid-auto-rows: minmax(10em, auto);
        justify-content: center;
    }
}
@media only screen and (min-width: 720px) {
    .proj-list-container {
        display: grid;
        grid-gap: 1em;
        grid-template-columns: repeat(3, minmax(100px, 300px));
        grid-auto-rows: minmax(10em, auto);
    }
}
</style>