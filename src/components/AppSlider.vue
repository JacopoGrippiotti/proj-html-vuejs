<template>
    <div class="slider">
        <h1>
            {{ slideList[activeIndex].title }} <span>{{ slideList[activeIndex].span }}</span>
        </h1>
        <p>{{ slideList[activeIndex].description }}</p>
        <input type="button" value="Get in Touch">
        
    </div>
</template>
<script>
export default {
    name:'AppSlider',
    props:{
        slideList:Array
    },
    data() {
        return {
            activeIndex:1
        }
    },
}
</script>
<style lang="scss" scoped>
    div.slider{
        width: 30%;
        margin: auto;
        text-align: center;

        h1{
            font-size: 72px;

            span{
                color: #058283;
            }
        }

        p{
            font-size: 19px;
            color: #606d75;
            font-weight: 400;
            margin-top: 30px;
        }

        input{
            padding: 10px 25px;
            text-transform: uppercase;
            font-size: 14px;
            background-color: #058283;
            border: 1px solid #058283;
            border-radius: 4px 4px 4px 4px;
            color: white;
            text-align: center;
            margin-top: 30px;
            margin-bottom: 30;
            &:hover{
                cursor: pointer;
            }
        }
    }
</style>