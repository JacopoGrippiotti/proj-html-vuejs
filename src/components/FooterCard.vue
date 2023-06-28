<template>
    <div class="footer-card">
        <h2>{{ title }}</h2>
        <ul>
            <li v-for="listItem in list">{{ listItem }}</li>
        </ul>
    </div>
</template>
<script>
export default {
    name:'FooterCard',
    props:{
        title:String,
        list:Array
    },
    data() {
        return {
           
        }
    },
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
    
    div.footer-card{
        width: calc(100% / 4) - 20px;
    }
</style>