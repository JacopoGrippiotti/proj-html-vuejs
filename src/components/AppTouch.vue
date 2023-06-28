<template>
    <section>
        <div class="container">
            <div class="left">
                <h4>send a message</h4>
                <h1>Get in <span>Touch</span></h1>
                <p>We will respond to your message as soon as possible</p>

                <form action="" method="get" class="form-example">
                  <div class="form-data">
                    <input type="text" name="name" id="name" placeholder="Name">
                    <input type="email" name="email" id="email" placeholder="Email">
                    <input type="text" name="phone" id="phone" placeholder="Phone">
                    <input type="select" name="info" id="info" placeholder="More info">
                    <input  class="area" type="textarea" name="message" id="message" placeholder="Message">
                    <input class="button" type="button" value="Send">
                  </div>
                
                </form>
            </div>
            <div class="right"></div>
        </div>
    </section>
</template>
<script>
export default {
    name:'AppTouch'
}
</script>
<style lang="scss" scoped>
    section{
        height: 900px;
    }
    div.container{
        width: 70%;
        margin: 0 auto;
        display: flex;

        div.left{
            width: 65%;

            form{
                display: flex;
                flex-direction: column;

                div.form-data{
                    display: flex;
                    flex-wrap: wrap;
                    justify-content: space-between;
                    input{
                        width:calc(50% - 10px);
                        background-color: rgb(236, 236, 236);
                        padding: 15px;
                        border-radius: 5px;
                        border: none;
                        margin-top: 10px;
                        font-size: 1rem;
                        color: rgb(90, 92, 94);
                    }

                    input.area{
                        width: 100%;
                        padding-bottom: 100px;
                    }

                    input.button{
                        padding: 10px 10px;
                        text-transform: uppercase;
                        font-size: 16px;
                        background-color: #058283;
                        border: 1px solid #058283;
                        border-radius: 4px 4px 4px 4px;
                        color: white;
                        text-align: center;
                        width: 10%;
                    }
                }

                

                   
                
            }
            h4{
                font-size: 16px;
                text-transform: uppercase;
                color: #058283;
                font-weight: 500;
            }

            h1{
                color: black;
                font-size: 48px;
                font-weight: 800;
                margin-top: 15px;

                span{
                    color: #058283;
                }
            }

            p{
                font-size: 1rem;
                font-weight: 400;
                color: #606D75;
            }
        }

        div.right{
            width: 35%;
        }
    }
</style>