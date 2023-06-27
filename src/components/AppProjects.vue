<template>
    <div class="container">
        <ProjectCard />
        
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
            cardList:
               {
                all:[{
                    title:'all'
                }],
                environment:[{
                    title:'environment'
                }],
                institutional:[{
                    title:'institutional'
                }],
                social:[{
                    title:'social'
                }],
                technology:[{
                    title:'technology'
                }],
                innovation:[{
                    title:'innovation'
                }],
                events:[{
                    title:'events'
                }],
            }
        }
    },
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
</style>