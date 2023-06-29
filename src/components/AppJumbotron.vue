<template>
    <section class="jumbotron">
        <AppSlider
        :slideList="slideList"/>
    </section>
</template>
<script>
import AppSlider from './AppSlider.vue';
export default {
    name:'AppJumbotron',
    components:{
        AppSlider
    },
    data() {
        return {
            slideList:[
                {
                    title:"We Share",
                    span:"Good Ideas",
                    description:"Escape the comfort zone and achieve better results with the help of experts who understand the subject"
                },
                {
                    title:"Ready",
                    span:"Team",
                    description:"No matter what your company needs, we will be ready to assist you in the best possible way."
                },
                {
                    title:"Talk to a",
                    span:"Consultant",
                    description:"Do not miss the opportunity to achieve better results and solidity in the market"
                }
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
    
    section.jumbotron{
        height: 1000px;
        background-image: url('../img/svgs/images/bg-parallax.png');
        display: flex;
        background-position-x:center ;
    }

    .background-center{
        background-position-x: center;
    }

    .background-right{
        background-position: right;
    }
    
</style>