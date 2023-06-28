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
        width: calc(100% / 4);
        background-color: rgb(25, 25, 31);
        color: white;
        justify-content: center;
        align-items: center;
        display: flex;
        flex-direction: column;
        padding: 20px 0px;
        border-radius: 7px;

        li{
            font-size: 15px;
            margin-top: 5px;
            color: rgb(174, 175, 182);
        }
    }
</style>