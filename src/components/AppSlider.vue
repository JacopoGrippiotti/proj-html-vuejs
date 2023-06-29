<template>
    <div class="slider">
        <h1>
            {{ slideList[activeIndex].title }} <span>{{ slideList[activeIndex].span }}</span>
        </h1>
        <p>{{ slideList[activeIndex].description }}</p>
        <input type="button" value="Get in Touch">
        <div class="inputs">
            <input type="button" @click="$emit('preSlide')">
            <input type="button" @click="$emit('centerSlide')">
            <input type="button" @click="$emit('rightSlide')">
        </div>
    </div>
</template>
<script>
export default {
    name:'AppSlider',
    props:{
        slideList:Array,
        activeIndex:Number
    },
    data() {
        return {
            
        }
    },
}
</script>
<style lang="scss" scoped>
    div.slider{
        width: 30%;
        margin: auto;
        text-align: center;
        

        div.inputs{
            position: absolute;
            display: flex;
            flex-direction: column;
            right: 30px;
            bottom: 50%;
            transform: translateY(50%);

            input{
                padding: 5px;
                margin-top: 10px;
            }
        }

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