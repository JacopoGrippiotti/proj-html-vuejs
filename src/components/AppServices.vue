<template>
    <div class="container light-gray">
        <div class="section-container">
            <h1>Excellence in services</h1>
            <div class="description">
                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
                <button>See All</button>
            </div>
            <div class="cardsContainer">
            <ServiceCard v-for="card in cardList"
            :title="card.title"
            :icon="card.icon" />
        </div>
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
        width: 100%;
        display: flex;
        padding: 40px 0px;
        
        div.section-container{
            margin: 0 auto;
            width: 70% ;
                
                div.description{
                    display: flex;
                    justify-content: space-between;
                    padding-top: 20px;
                    p{
                        width: 70%;
                    }
                }
                div.cardsContainer{
                margin: 0 auto;
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
                }
        }
        
    }
</style>