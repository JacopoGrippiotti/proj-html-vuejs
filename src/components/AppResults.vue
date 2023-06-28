<template>
    <section>
        <div class="chess">
            <div class="numbers-container">
                <h4>What are we doing</h4>
                <h1>Results in Numbers</h1>
                <ul>
                    <li>
                        <span class="number">128</span>
                        <span class="title">Certifications</span>
                    </li>
                    <li>
                        <span class="number">230</span>
                        <span class="title">Employees</span>
                    </li>
                    <li>
                        <span class="number">517</span>
                        <span class="title">Customers</span>
                    </li>
                    <li>
                        <span class="number">94</span>
                        <span class="title">Countries Served</span>
                    </li>
                </ul>
            </div>
        </div>
        <div class="program-languages">
            <div class="languages-container">
                <ul>
                  <li>
                    <img src="../img/svgs/images/logo-4.png" alt="">
                  </li>
                  <li>
                    <img src="../img/svgs/images/logo-5.png" alt="">
                  </li>
                  <li>
                    <img src="../img/svgs/images/logo-1.png" alt="">
                  </li>
                  <li>
                    <img src="../img/svgs/images/logo-2.png" alt="">
                  </li>
                  <li>
                    <img src="../img/svgs/images/logo-3.png" alt="">
                  </li>
                  <li>
                    <img src="../img/svgs/images/logo-4.png" alt="">
                  </li>
                </ul>
            </div>
            
        </div>
    </section>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    @use '../styles/partials/mixins.scss' as*;
    @use '../styles/partials/variables.scss' as*;

    section{
        width: 100%;
        display: flex;
        flex-direction: column;

        div.chess{
            padding: 110px 0px;
            width: 100%;
            background-image: url("../img/svgs/images/bg-7.jpg");
            background-position: center;
            display: flex;
            align-items: center;
            

            div.numbers-container{
                width: 60%;
                margin: 0 auto;
                text-align: center;

                h4{
                   font-size: 16px;
                   text-transform: uppercase;
                   color: #058283;
                   font-weight: 500;
                }

                h1{
                    color: white;
                    font-size: 48px;
                    font-weight: 800;
                    margin-top: 30px;
                }
                
                ul{
                    display: flex;
                    justify-content: space-between;
                    color: white;
                    padding-top: 130px;

                    li{
                        display: flex;
                        flex-direction: column;
                        align-items: center;

                        span.number{
                            color: rgb(38, 166, 166);
                            font-size: 27px;
                            font-weight: 700;
                        }

                        span.title{
                            font-size: 20px;
                            font-weight: 700;
                            margin-top: 20px;
                        }
                    }
                }
            }
        }

        div.program-languages{
            
            background-color: black;
            width:100%;
            display: flex;
            align-items: center;
            div.languages-container{
                width: 60%;
                margin: 0 auto;
                
                ul{
                    display: flex;
                    justify-content: space-between;
                    align-items: center;
                    padding: 50px 0px;

                    
                    img{
                        width: 80px;
                        filter: brightness(3);
                    }
                }
            }

        }
    }
</style>