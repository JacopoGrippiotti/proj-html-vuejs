<template>
    <div class="cardService white-gray">
        <img :src="getIcon(icon)" alt="">
        <h2>{{ title }}</h2>
    </div>
</template>
<script>
export default {
    name:'ServiceCard',
    props:{
        title:String,
        icon:String
    },
    methods: {
        getIcon(icon){
            return new URL (`${icon}`, import.meta.url).href;
        }
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/general.scss' as*;
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;

    div.cardService{
        width:calc((100% / 3) - 30px);
        padding: 35px;
        margin-top: 40px;

        h2{
            font-size: 1.5rem;
            font-weight: 700;
            color: #21333e;
        }
        img{
            height: 45px;
            width: 45px;
            filter: brightness(0) saturate(100%) invert(25%) sepia(75%) saturate(2664%) hue-rotate(163deg) brightness(93%) contrast(96%);
        }
    }
</style>