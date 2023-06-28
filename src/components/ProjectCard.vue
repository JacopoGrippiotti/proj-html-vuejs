<template>
    <div class="cardProject">
        <img :src="getBackground(path)" alt="">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
    </div>
</template>

<script>
export default {
    name:'ProjectCard',
    props:{
        path:String
    },
    methods: {
        getBackground(path){
            return new URL (`${path}`, import.meta.url).href;
        }
    }
}
</script>

<style lang="scss" scoped>
    @use '../styles/general.scss' as*;
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
    div.cardProject{
        width: calc((100% / 3) - 23px );
        height: 300px;
        margin-top: 30px;
        position: relative;
        
        img{
            height: 100%;
            width: 100%;
            border-radius: 6px 6px 6px 6px;
        }

        p{
            position: absolute;
            color: white;
            bottom: 30px;
            font-size: 20px;
            font-weight: 700;
        }
    }
</style>