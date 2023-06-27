<template>
   <section class="projects">
    <h1>Actions & <span>Projects</span></h1>
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
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;

    section.projects{
        text-align: center;
        
        h1{
            margin-bottom: 24px;
            font-size: 48px;
            font-weight: 800
        }

        span{
            color: #058283
        }
        div.container{
        width: 70%;
        height: 900px;
        background-color: white;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        margin: 0 auto;
    }
    }
</style>