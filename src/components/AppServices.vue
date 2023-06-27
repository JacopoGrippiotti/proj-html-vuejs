<template>
    <div class="container light-gray">
        <div class="cardsContainer">
          <ServiceCard/>
        </div>
    </div>
    
</template>
<script>
import ServiceCard from './ServiceCard.vue';
export default {
    name:'AppServices',
    components:{
        ServiceCard
    }
}
</script>
<style lang="scss" scoped>
   @use '../styles/general.scss' as*;
   @use '../styles/partials/mixins.scss' as*;
   @use '../styles/partials/variables.scss' as*;
    div.container{
        height: 800px;
        width: 100%;
        display: flex;
        padding: 40px 0px;
        
        div.cardsContainer{
            width: 70%;
            margin: 0 auto;
            background-color: blue;
            
        }
    }
</style>