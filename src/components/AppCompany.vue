<template>
    <section>
        <div class="container">
          <div class="description">
            <h1>The Company</h1>
          </div>
          <div class="image"> 

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
    }
    div.container{
        height: 659px;
        display: flex;
        padding: 100px 0px;
        width: 70%;
        margin: 0 auto;
       
        div.description{
            width: 40%;
            
            h1{
                font-size: 48px;
                color: white;
            }
        }

        div.image{
            width: 40%;
        }
       
    }
</style>