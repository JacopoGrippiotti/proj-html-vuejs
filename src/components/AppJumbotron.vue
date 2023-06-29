<template>
    <section class="jumbotron" :class="slideList[activeIndex].background">
        <AppSlider
        :slideList="slideList"
        :activeIndex="activeIndex"
        @preSlide="preSlide"
        @centerSlide="centerSlide"
        @rightSlide="rightSlide"/>
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
                    description:"Escape the comfort zone and achieve better results with the help of experts who understand the subject",
                    background:"background-left"
                },
                {
                    title:"Ready",
                    span:"Team",
                    description:"No matter what your company needs, we will be ready to assist you in the best possible way.",
                    background:"background-center"
                },
                {
                    title:"Talk to a",
                    span:"Consultant",
                    description:"Do not miss the opportunity to achieve better results and solidity in the market",
                    background:"background-right"
                }
            ],
            activeIndex:1
        }
    },
    methods:{
        preSlide(){
            if(this.activeIndex === 0){
                return false
            }

            if(this.activeIndex === 1){
                this.activeIndex = this.activeIndex - 1
            }
            if(this.activeIndex === 2){
                this.activeIndex = this.activeIndex - 2
            }
            
            
        },
        centerSlide(){
            if(this.activeIndex === 1){
                return false
            }

            if(this.activeIndex === 0){
                this.activeIndex = this.activeIndex + 1
            }
            
            if(this.activeIndex === 2){
                this.activeIndex = this.activeIndex - 1
            }
            
        },
        rightSlide(){
            if(this.activeIndex === 2){
                return false
            }
            this.activeIndex = this.activeIndex + 1
        }
    }
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;
    
    section.jumbotron{
        height: 1000px;
        background-image: url('../img/svgs/images/bg-parallax.png');
        display: flex;
        transition: background-position-x 1.2s ease-in-out;
        position: relative;
    }

    .background-center{
        background-position-x: center;
    }

    .background-right{
        background-position-x: right;
    }

    .background-left{
        background-position-x: left;
    }
    
</style>