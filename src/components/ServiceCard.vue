<template>
    <div class="cardService">
        <img src="" alt="">
    </div>
</template>
<script>
export default {
    name:'ServiceCard',
    props:{
        title:String,
        icon:String
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;

    div.cardService{
        width:calc((100% / 3) - 30 px);
        padding: 20px 15px;
    }
</style>