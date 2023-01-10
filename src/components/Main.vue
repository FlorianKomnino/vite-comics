<script>
import ComicsObject from '../json/dc-comics.json';


export default {
    components: {
        ComicsObject,
    }
}
</script>

<template>
    <div class="contentGoesHere">
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron image">
        </div>
    </div>

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

div.contentGoesHere,
div.blueBar {
    width: 100%;
    margin: 0 auto;
    padding: 0;
    display: flex;
    justify-content: center;
}
</style>
