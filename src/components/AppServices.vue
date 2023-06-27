<template>
    <div class="container light-gray">
        <div class="cardsContainer">
          <ServiceCard 
          :cardList="cardList" />
        </div>
    </div>
    
</template>
<script>
import ServiceCard from './ServiceCard.vue';
export default {
    name:'AppServices',
    components:{
        ServiceCard
    },
    data() {
        return {
            cardList:[{
                title:'Audit & Assurance',
                icon:'../img/svgs/svg-1.svg'
            },
            {
                title:'Financial Advisory',
                icon:'../img/svgs/svg-2.svg'
            },
            {
                title:'Analytics and M&A',
                icon:'../img/svgs/svg-3.svg'
            },
            {
                title:'Middle Marketing',
                icon:'../img/svgs/svg-4.svg'
            },
            {
                title:'Legal Consulting',
                icon:'../img/svgs/svg-5.svg'
            },
            {
                title:'Regulatory Risk',
                icon:'../img/svgs/svg-6.svg'
            }
            ]
        }
    },

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