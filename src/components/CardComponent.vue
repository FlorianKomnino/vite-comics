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
        <img :src="imagePath" alt="comic wallpaper">
        <h6 class="serie"></h6>
    </div>
</template>


<style scoped>
div.comicElement {
    height: 130px;
    width: 130px;
}

h6.serie {
    color: white;
}
</style>
