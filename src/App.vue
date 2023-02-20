<template>
  <div>
    <NavBar :logo ="logo_src" :alt="app_name"/>
    <router-view></router-view>
    <Footer></Footer>
  </div>
</template>


<script>
  import NavBar from './components/NavBar.vue'
  import Footer from './components/Footer.vue'

  export default{
    name:'App',
    components:{
      NavBar,Footer
    },
    data(){
      return{
        logo_src: "/img/logo.png",
        app_name: "Make Your Burguer"
      }
    }
  }

</script>

<style>
  *{
    font-family: Arial, Helvetica, sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-conteiner{
    margin: 50px;
    min-height: 250px;
  }

  h1{
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>
