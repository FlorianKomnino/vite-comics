<script>

</script>

<template>
    <div class="outerContainer">

        <div class="innerContainer">
            <div class="primary-logo">
                <figure>
                    <img src="../assets/img/dc-logo.png" alt="DC Logo">
                </figure>
            </div>

            <nav>
                <ul>
                    <li>characters</li>
                    <li>characters</li>
                    <li>characters</li>
                    <li>characters</li>
                    <li>characters</li>
                    <li>characters</li>
                </ul>
            </nav>
        </div>
    </div>

</template>

<style scoped>
nav {
    display: flex;
}

ul {
    margin: auto 0;
    display: flex;
}

li {
    padding: 10px;
}

img {
    height: 80%;
    margin: auto;
}

figure {
    height: 100%;
    display: flex;
}

div.primary-logo {
    height: 70px;
}

.outerContainer {
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.innerContainer {
    justify-content: space-between;
}
</style>
