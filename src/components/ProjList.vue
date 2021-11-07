<template>
    <div>
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
                    id: 'dd264b69f8362ee106f25f11b13a46f7',
                    title: "Emblica",
                    desc: "a React app to learn English",
                    link: "https://emblica.herokuapp.com/",
                    date: "2020",
                    image: "emblica.png",
                    for: "my wife",
                },
                {
                    id: '6b2985034a01f2fcf9d2836a2dec12e1',
                    title: "Dragonfruit",
                    desc: "a React app to learn Spanish",
                    link: "https://dragonfruit.herokuapp.com/",
                    date: "2020",
                    image: "dragonfruit.png",
                    for: "myself",
                },
                {
                    id: '16db7ef414f27c5d54ce976c7710695a',
                    title: "Expensify",
                    desc: "a React app",
                    link: "https://igoryen-expensify.herokuapp.com/",
                    date: "2020",
                    image: "expensify.png",
                    for: "myself",
                },
                {
                    id: '18fe7347ac4e04e020d963ce0a1a060d',
                    title: "NAS Mobile App",
                    desc: "UI by me",
                    link:
                        "https://apps.apple.com/ca/app/valuation-mobile-app/id536228581#?platform=iphone",
                    date: "2019",
                    image: "nas.png",
                    for: "the Nationwide Group",
                },
                {
                    id: '7399d3d109ecf848fb597ffe14fa8101',
                    title: "CNX",
                    desc: "Brochure website",
                    link: "https://www.connexionssoftware.com/",
                    date: "2019",
                    image: "cnx.png",
                    for: "the Nationwide Group",
                },
                {
                    id: '3cf3d57a138fb0d0aba3e9eb42582dce',
                    title: "NRS",
                    desc: "Brochure site, bilingual",
                    link: "https://www.nwrs.ca/",
                    date: "2018",
                    image: "nrs.png",
                    for: "the Nationwide Group",
                },
                {
                    id: '404bb491f26ee6cbdf99e19d4b031c42',
                    title: "HCS",
                    link: "https://nwhcs.ca/",
                    desc: "Static website, improved by me (WIP)",
                    date: "2018",
                    image: "hcs.png",
                    for: "the Nationwide Group",
                },
                {
                    id: 'a1de9672c054b2c64b78186bce19a639',
                    title: "NAS",
                    link: "https://www.nationwideappraisals.com/NAS/index.jsp",
                    desc: "Multiple pages, design implementation",
                    date: "2018",
                    image: "nas-site.png",
                    for: "the Nationwide Group",
                },
                {
                    id: '41db778118898f2eab767fbfde3bff48',
                    title: "Lexus.ca",
                    desc: "Multiple pages, design implementation",
                    link: "https://www.lexus.ca/lexus/en",
                    date: "2015-2016",
                    image: "lexus.png",
                    for: "Saatchi & Saatchi",
                },
                {
                    id: 'c4a3a9d6ffe80616f3ba1c95b68fe81b',
                    title: "Toyota.ca",
                    desc: "Multiple pages, design implementation",
                    link: "https://www.toyota.ca/toyota/en/",
                    date: "2015-2016",
                    image: "toyota.png",
                    for: "Saatchi & Saatchi",
                },
                {
                    id: '80fcc9264ecdb6e0287699b4c43b3e53',
                    title: "Mozilla Webmaker",
                    desc: "Localization, backend",
                    link: "https://foundation.mozilla.org/en/artifacts/webmaker/",
                    date: "2013",
                    image: "mozilla-webmaker.jpg",
                    for: "Mozilla",
                },
                {
                    id: '3befde5a4ab44fecf9d926b3643b5870',
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