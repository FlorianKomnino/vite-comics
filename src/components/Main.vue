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

            blueBarList: [
                'digital comicas',
                'dc merchandise',
                'subscription',
                'comic shop locator',
                'dc power visa',
            ],
        }
    }
}
</script>

<template>
    <div class="topMain">
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
        <div class="innerContainer">
            <button>load more</button>
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

button {
    padding: 0.5rem 3rem;
    color: white;
    background-color: #0282f9;
    font-weight: 600;
    text-transform: uppercase;
    font-size: 0.75rem;
}

div.jumbotron {
    overflow: hidden;

    img {
        width: 100%;
    }
}

div.topMain {
    background-color: #1c1c1c;
    height: 350px;
}

div.blueBar {
    background-color: #0282f9;
    height: 150px;
}

section.comicsWrapper {
    color: white;
    background-color: #1c1c1c;

    .innerContainer {
        position: relative;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        padding: 3rem 0;
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

section.comicsWrapper {
    width: 100%;
    margin: 0 auto;
    padding: 0;
}

div.topMain,
div.blueBar {
    width: 100%;
    margin: 0 auto;
    padding: 0;
    display: flex;
    justify-content: center;
}
</style>
