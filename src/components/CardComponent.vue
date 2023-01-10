<script>
export default {
    name: 'CardComponent',
    props:
    {
        imagePath: String,
        serie: String,
        price: { type: Number, required: false },
        comicType: { type: String, required: false },
    },
}
</script>


<template>
    <div class="comicElement">
        <figure>
            <img :src="imagePath" alt="comic wallpaper">
        </figure>
        <h5 class="serie">{{ serie }}</h5>
    </div>
</template>


<style lang="scss" scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

div.comicElement {
    height: 175px;
    width: (calc(100% / 6) - 4);
    margin: 1rem;

    figure {
        overflow: hidden;
        width: 100%;
        height: 100%;
    }

    img {
        margin-top: 1rem;
        width: 100%;
    }
}

h5.serie {
    padding: 1rem 0;
    color: white;
    text-transform: uppercase;
    font-weight: 400;
    font-size: 0.75rem;
    ;
}
</style>
