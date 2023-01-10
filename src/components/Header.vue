<script>
export default {
    data() {
        return {
            dcComics: {
                title: 'dc comics',
                list: [
                    'characters',
                    'comics',
                    'movies',
                    'TV',
                    'games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop',
                ]
            },
        }
    }
}
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
                    <li v-for="listItem, index in dcComics.list">{{ dcComics.list[index] }}</li>
                </ul>
            </nav>
        </div>
    </div>

</template>

<style lang="scss" scoped>
nav {
    display: flex;
}

ul {
    height: 100%;
    display: flex;
    align-items: center;
}

li {
    height: 100%;
    padding: 2rem 10px;
    font-size: 0.9rem;
    font-weight: 600;
    text-transform: uppercase;
    border-bottom: 2px solid transparent;

    &:hover {
        border-bottom: 2px solid #0282f9;
        color: #0282f9;
    }
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
