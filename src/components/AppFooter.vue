<template>
    <footer>
        <div class="container">

          <div class="card">
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
                    
                    <input type="button" value="get in touch">
            </ul>
          </div>
          <FooterCard v-for="card in menuList"
           :title="card.title" :list="card.listItems"/>
        </div>
    </footer>
    
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

    footer{
        background-color: rgb(17, 17, 23);
        padding: 120px 0px;
        div.container{
            margin: 0 auto;
            width: 70%;
            display: flex;
            justify-content: space-between;

            div.card{
                width: calc((100% / 4) - 20px );

                ul{
                display: flex;
                flex-direction: column;

                li{
                    display: flex;
                    align-items: baseline;
                    margin-top: 7px;
                    

                    i{
                     color: rgb(174, 175, 182);
                     font-size: 1.2rem;   
                    }
                    
                    span{
                        color: rgb(174, 175, 182);
                        margin-left: 10px;
                    }

                    
                }
            }
                    input{
                        padding: 10px;
                        text-transform: uppercase;
                        font-size: 14px;
                        background-color: black;
                        border: 1px solid #058283;
                        border-radius: 4px 4px 4px 4px;
                        color: #058283;
                        margin-top: 30px;
                        margin-bottom: 30px;
                        width: 50%;
                    }
            }
        }
    }
</style>