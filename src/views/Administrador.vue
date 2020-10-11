<template>
  <div>
    <header class="masthead" style="background-image:url('assets/img/about-bg.jpg');">
    <div class="overlay"></div>
    <div class="container">
        <div class="row">
            <div class="col-md-10 col-lg-8 mx-auto">
                <div class="site-heading">
                    <h1><strong>{{title}}</strong></h1>
                </div>
            </div>
        </div>
    </div>
</header>
  </div>
</template>

<script>
export default {

    props:{
        admin:{
            type: String
        }
    },
    computed:{
        title(){
           if(this.admin == 'simple'){
               return 'Hola Mundo'
           }else if(this.admin == 'avanzado'){
               return 'hola'
           }else{
               return ""
           }
        }
    }
}
</script>

<style>

</style>