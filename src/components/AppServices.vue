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
    div.container{
        height: 1037px;
        width: 100%;
        display: flex;
    }
</style>