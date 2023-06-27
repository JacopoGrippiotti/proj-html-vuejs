<template>
    <div class="cardService white-gray">
        <div class="images-container">
            <img :src="getIcon(icon)" alt="">
            <i class="fa-solid fa-arrow-right"></i>
        </div>
        <h2>{{ title }}</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
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
        border-radius: 0.25rem;

       div.images-container{
        display: flex;
        justify-content: space-between;
        font-size: 1.7rem;
        color: #058283;
       }

        p{
            width: 100%;
            font-size: 1rem;
            font-weight: 400;
            color: #606D75;
            padding-top: 25px;
        }
        
        h2{
            font-size: 1.5rem;
            font-weight: 700;
            color: #21333e;
            padding-top: 25px;
        }
        
        img{
            height: 45px;
            width: 45px;
            filter: brightness(0) saturate(100%) invert(25%) sepia(75%) saturate(2664%) hue-rotate(163deg) brightness(93%) contrast(96%);
        }
    }
</style>