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
        <h6 class="serie">{{ serie }}</h6>
    </div>
</template>


<style lang="scss" scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

div.comicElement {
    height: 130px;
    width: (calc(100% / 6) - 4);
    margin: 1rem;

    figure {
        overflow: hidden;
        width: 100%;
        height: 100%;
    }

    img {
        width: 100%;
    }
}

h6.serie {
    color: white;
}
</style>
