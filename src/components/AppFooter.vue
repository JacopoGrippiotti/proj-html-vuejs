<template>
    <section>
        <div class="container">
        <FooterCard v-for="card in menuList"
        :title="card.title" :list="card.listItems"/>
        </div>
    </section>
    
</template>
<script>
import FooterCard from './FooterCard.vue';
export default {
    name:'AppFooter',
    components:{
        FooterCard
    },
    data() {
        return {
            menuList:[
                     {
                      title:"About",
                      listItems:["The Company","Institutional","Social & Events","Innovation","Environment","Technology"]
                     },
                     {
                      title:"Services",
                      listItems:["Audit & Assurance","Financial Advisory","Analytics M&A","Middle Marketing","Legal Consulting","Regulatory Risk"]
                     },
                     {
                      title:"Support",
                      listItems:["Responsibility","Terms of Use","About Cookies","Privacy Policy","Accessibility","Information"]
                     }
                ]
        }
    },
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
</style>