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
        width: calc((100% / 3) - 30px );
        
        img{
            height: 300px;
        }
    }
</style>