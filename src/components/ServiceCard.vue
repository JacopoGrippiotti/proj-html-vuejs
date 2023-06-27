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
        padding: 20px 15px;
        margin-top: 40px;
        img{
            height: 30px;
            width: 30px;
        }
    }
</style>