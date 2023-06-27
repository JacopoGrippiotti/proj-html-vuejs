<template>
    <section>
        <div class="container">
          <div class="description">
            <h1>The Company</h1>
            <p>For 12 years  we have been providing audit and warranty, financial advice, taxes and related services to select clients.</p>
            <div class="cards-slider">
                <div class="card">
                    <i class="fa-solid fa-award"></i>
                    <span>Tradition</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>
                
                <div class="card">
                    <i class="fa-solid fa-lock"></i>
                    <span>Security</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>
                
                <div class="card">
                    <i class="fa-regular fa-pen-to-square"></i>
                    <span>Certificate</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>
                
                <div class="card">
                    <i class="fa-solid fa-user-tie"></i>
                    <span>Expertise</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>

                <div class="buttons-wrapper">
                    <input  type="button" value="get in touch">
                    <input  class="black" type="button" value="read more" >
                </div>
                
            </div>
          </div>
          <div class="images"> 
            <div class="wrapper">
                <div class="parallax">

                </div>
            </div>
          </div>
        </div>
    </section>
</template>
<script>
export default {
    name:'AppCompany'
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;

    section{
        background-color:rgb(17, 17, 23);
        position: relative;
        width: 100%;
    }
    div.container{
        display: flex;
        padding: 100px 0px;
        width: 70%;
        margin: 0 auto;
       
        div.description{
            width: 50%;
        
            h1{
                font-size: 48px;
                color: white;
            }

            p{
            width: 100%;
            font-size: 16px;
            font-weight: 400;
            color: #AFB6BA;
            padding-top: 25px;
            }

            div.cards-slider{
                width: 100%;
                display: flex;
                flex-wrap: wrap;
                padding-top: 20px;
                
                    div.card{
                    width: 50%;
                    margin-top: 25px;

                    i{
                        font-size: 25px;
                        color: #00A6A6;
                    }
                    
                    span{
                        font-size: 24px;
                        color: white;
                        font-weight: 700;
                        padding-left: 10px;
                    }
                    }

                    div.buttons-wrapper{
                        width: 100%;
                        display: flex;
                        margin-top: 70px;
                        
                        input{
                            padding: 10px 25px;
                            text-transform: uppercase;
                            font-size: 16px;
                            background-color: #058283;
                            border: 1px solid #058283;
                            border-radius: 4px 4px 4px 4px;
                            color: white;
                            margin-right: 20px;
                        }

                        input.black{
                            background-color: black;
                            border:1px solid #058283;
                        }
                    }
            }
        }

        div.images{
            width: 50%;

            div.wrapper{
                height: 100%;
                width: 100%;
                div.parallax {
                background-image: url("../img/svgs/images/about-4.jpg");
                background-attachment: scroll;
                background-repeat: no-repeat;
                
                background-size: cover;
                height: 100%;
                width: 50%;
                position: absolute;
                bottom: 0;
                }
            }
            

        }
            
        
       
    }
</style>