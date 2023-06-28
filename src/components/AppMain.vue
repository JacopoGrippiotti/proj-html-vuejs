<template>
    <AppJumbotron/>
    <AppServices/>
    <AppCompany/>
    <AppProjects/>
    <AppResults/>
    <AppTouch/>
</template>
<script>
 import AppJumbotron from './AppJumbotron.vue';
 import AppServices from './AppServices.vue';
 import AppCompany from './AppCompany.vue';
 import AppProjects from './AppProjects.vue';
 import AppResults from './AppResults.vue';
 import AppTouch   from './AppTouch.vue';
 
export default {
    name:'AppMain',
    components:{
        AppJumbotron,
        AppServices,
        AppCompany,
        AppProjects,
        AppResults,
        AppTouch
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
</style>