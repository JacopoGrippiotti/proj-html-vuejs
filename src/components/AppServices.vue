<template>
    <div class="container light-gray">
        <div class="section-container">
            <h1>Excellence in 
                <span>Services</span>
            </h1>
            <div class="description">
                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
                <input type="button"  value="See All">
                
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
        
        
        div.section-container{
            margin: 0 auto;
            width: 70% ;
            padding: 80px 0px;
                
                h1{
                    margin-bottom: 24px;
                    font-size: 48px;
                    font-weight: 800
                    
                    
                }

                span{
                    color: #058283;
                }
                
                div.description{
                    display: flex;
                    justify-content: space-between;
                    p{
                        width: 75%;
                        font-size: 1rem;
                        font-weight: 400;
                        color: #606D75;
                    }

                    input{
                        padding: 10px 25px;
                        text-transform: uppercase;
                        font-size: 16px;
                        background-color: #058283;
                        border: none;
                        border-radius: 4px 4px 4px 4px;
                        color: white;
                    }
                }
                div.cardsContainer{
                margin: 0 auto;
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
                margin-top: 13px;
                }
        }
        
    }
</style>