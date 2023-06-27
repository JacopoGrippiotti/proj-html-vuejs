<template>
    <section>
        <div class="container">
          <div class="description">
            <h1>The Company</h1>
            <p>For 12 years  we have been providing audit and warranty, financial advice, taxes and related services to select clients.</p>
            <div class="cards-container">
                <div>
                    <i class="fa-solid fa-hourglass-end"></i>
                    <span>Tradition</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>
                
                <div>
                    <i class="fa-solid fa-lock"></i>
                    <span>Security</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>
                
                <div>
                    <i class="fa-solid fa-apple-whole"></i>
                    <span>Certificate</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
                </div>
                
                <div>
                    <i class="fa-solid fa-user-tie"></i>
                    <span>Expertise</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
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
        background: linear-gradient(45deg, rgb(13, 27, 42), rgb(34, 72, 100));
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

            div.cards-container{
                width: 100%;
                display: flex;
                flex-wrap: wrap;
                padding-top: 20px;
                
                    div{
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