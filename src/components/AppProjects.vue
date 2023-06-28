<template>
   <section class="projects">
    <h4>We do more for everyone</h4>
    <h1>Actions & <span>Projects</span></h1>
    <ul>
        <li v-for="name in listTypes"> {{ name }} </li>
    </ul>
    <div class="container">
        <ProjectCard 
        :path="card.path" v-for="card in cardList"/>
    </div>
   </section>
    
</template>
<script>
import ProjectCard from './ProjectCard.vue';
export default {
    name:'AppProjects',
    components:{
        ProjectCard
    },
    data() {
        return {
            cardList:[
                {   
                    title:'All',
                    name:'academic',
                    path:'../img/svgs/images/project-1.jpg',
                    description:'Academic professional program in social media'                                         
                },
                {
                    title:'institutional',
                    name:'president',
                    path:'../img/svgs/images/project-2.jpg',
                    description:'President s speech at the annual meeting'                     
                },
                {
                    title:'social',
                    name:'business',
                    path:'../img/svgs/images/project-3.jpg',
                    description:'International business trip in Shangai'                     
                },
                {
                    title:'events',
                    name:'technology',
                    path:'../img/svgs/images/project-4.jpg',
                    description:'Technology workshop with education theme'
                },
                {
                    title:'innovation',
                    name:'donation',
                    path:'../img/svgs/images/project-5.jpg',
                    description:'Donation of clothes and food  to the partner NGO'
                },
                {
                    title:'environment',
                    name:'social',
                    path:'../img/svgs/images/project-6.jpg',
                    description:'Confraternization of the procurement team'
                },
            ],
            listTypes:["all","institutional","social","events","innovation","environment","technology"]
        }
    },
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;

    section.projects{
        text-align: center;
       
       
        
        ul{
            display: flex;
            justify-content: space-evenly;
            width: 70%;
            margin: 0 auto;
            margin-top: 50px;

            li{
                text-transform: uppercase;
            }
        }

        h4{
            font-size: 16px;
            text-transform: uppercase;
            color: #058283;
            font-weight: 500;
            margin-top: 120px;
        }
        h1{
            margin-bottom: 24px;
            font-size: 48px;
            font-weight: 800;
            margin-top: 20px;
        }

        span{
            color: #058283
        }
        div.container{
        width: 70%;
        background-color: white;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        margin: 0 auto;
        padding-bottom: 120px;
    }
    }
</style>