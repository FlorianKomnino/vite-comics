<script>
import comicsArray from '../json/dc-comics.json';
import CardComponent from './CardComponent.vue';

export default {
    components: {
        CardComponent,
    },

    data() {
        return {
            comics: comicsArray,
        }
    }
}
</script>

<template>
    <div class="contentGoesHere">
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron image">
        </div>
    </div>

    <section class="comicsWrapper">
        <div class="innerContainer">
            <div class="sectionTitle">
                <h1>
                    current series
                </h1>
            </div>

            <CardComponent v-for="comic in comics" :imagePath="comic.thumb" :serie="comic.series" />

        </div>
    </section>

    <div class="blueBar">
        <div class="innerContainer">
            <h2>
                Blue Bar content goes here
            </h2>
        </div>
    </div>

</template>

<style lang="scss" scoped>
figure {
    height: 100%;
    display: flex;
}

h2 {
    color: white;
    margin: auto 0;
}

div.jumbotron {
    overflow: hidden;

    img {
        width: 100%;
    }
}

div.contentGoesHere {
    background-color: #1c1c1c;
    height: 350px;
}

div.blueBar {
    background-color: #0282f9;
    height: 150px;
}

section.comicsWrapper {
    color: white;
    height: 300px;
    background-color: #1c1c1c;

    .innerContainer {
        position: relative;
    }
}

.innerContainer .sectionTitle {
    position: absolute;
    top: -10px;
    left: 0;
    background-color: #0282f9;
    padding: 0.5rem;
    text-transform: uppercase;
}


section.comicsWrapper,
div.contentGoesHere,
div.blueBar {
    width: 100%;
    margin: 0 auto;
    padding: 0;
    display: flex;
    justify-content: center;
}
</style>
