<script>
export default {
    data() {
        return {
            imageName: "wallpaper.jpg"
        }
    },
    methods: {
        getImagePath: function (img) {
            return new URL(`../assets/img/${img}`,import.meta.url).href;
        }
    },
}
</script>

<template>
    <div class="flex">
        <img :src="getImagePath(imageName)" class="img_style">
    </div>
</template>

<style>
.img_style {
width: 100%;
border-radius: 50px;
box-shadow: 5px 10px 8px #888888;
}


</style>

