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
            <div class="right">
                <h2>Example Inc.</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                <p>Praesent diam lacus, dapibus sed imperdiet consectetur.</p>
                <ul>
                    <li>
                        <div class="icon">
                            <i class="fa-solid fa-phone"></i>
                        </div>
                        
                        <span>+1 (305) 1234-5678</span>
                    </li>
                    <li>
                        <div class="icon">
                            <i class="fa-solid fa-envelope"></i>
                        </div>
                        
                        <span>hello@example.com</span>
                    </li>
                    <li>
                        <div class="icon">
                            <i class="fa-solid fa-location-dot"></i>
                        </div>
                        
                        <span>Main Avenue, 987</span>
                    </li>
                    
                </ul>
                <input type="button" value="View map">
            </div>
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
        padding: 120px 0px;
    }
    div.container{
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;

        div.left{
            width: 65%;

            form{
                display: flex;
                flex-direction: column;
                margin-top: 40px;

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
                        font-size: 14px;
                        background-color: #058283;
                        border: 1px solid #058283;
                        border-radius: 4px 4px 4px 4px;
                        color: white;
                        text-align: center;
                        width: 10%;
                        margin-top: 30px;
                        margin-bottom: 30px;
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
                color: rgb(125, 134, 139);
                margin-top: 20px;
            }
        }

        div.right{
            width: 32%;
            ul{
                display: flex;
                flex-direction: column;

                li{
                    display: flex;
                    align-items: baseline;

                    span{
                       color: #058283;
                       margin-left: 10px;
                    }
                }
            }

            input{
                padding: 10px 10px;
                text-transform: uppercase;
                font-size: 14px;
                background-color: white;
                border: 1px solid #058283;
                border-radius: 4px 4px 4px 4px;
                color: #058283;
                margin-top: 30px;
                margin-bottom: 30px;
            }
            p{
                font-size: 1rem;
                font-weight: 400;
                color: rgb(125, 134, 139);
                margin-top: 20px;
            }

            div.icon{
                height: 40px;
                width: 40px;
                background-color: rgb(219, 236, 237);
                display: flex;
                border-radius: 50%;
                margin-top: 30px;

                i{
                color: #058283;
                margin:  auto;
                font-size: 1.2rem;   
            }
            }

            
        }
    }
</style>