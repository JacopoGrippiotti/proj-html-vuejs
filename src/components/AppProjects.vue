<template>
    <div class="container">
        <ProjectCard 
        :path="path" v-for="card in cardList"/>
    </div>
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
                    name:'academic',
                    path:'../img/svgs/images/project-1.jpg',
                    description:'Academic professional program in social media'                                         
                },
                {
                    name:'president',
                    path:'../img/svgs/images/project-2.jpg',
                    description:'President s speech at the annual meeting'                     
                },
                {
                    name:'business',
                    path:'../img/svgs/images/project-3.jpg',
                    description:'International business trip in Shangai'                     
                },
                {
                    name:'technology',
                    path:'../img/svgs/images/project-4.jpg',
                    description:'Technology workshop with education theme'
                },
                {
                    name:'donation',
                    path:'../img/svgs/images/project-5.jpg',
                    description:'Donation of clothes and food  to the partner NGO'
                },
                {
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
</style>