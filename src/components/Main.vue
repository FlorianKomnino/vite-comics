<script>

</script>

<template>
    <div class="contentGoesHere">
        <div class="innerContainer">
            <h2>
                Content goes here
            </h2>
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

<style scoped>
div.contentGoesHere {
    background-color: #1c1c1c;
}

div.blueBar {
    background-color: #0282f9;
}

div.contentGoesHere,
div.blueBar {
    width: 100vw;
    height: 130px;
    margin: 0 auto;
    padding: 0;
    display: flex;
}

h2 {
    color: white;
    margin: auto 0;
}
</style>
