<template>
    <div class="container">
        <ProjectCard/>
    </div>
</template>
<script>
import ProjectCard from './ProjectCard.vue';
export default {
    name:'AppProjects',
    components:{
        ProjectCard
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
</style>