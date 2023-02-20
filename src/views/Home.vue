<template>
  <div class="main-conteiner">
    <Banner/>
    <h1>Monte seu burger:</h1>
    <FormBurger/>
  </div>
</template>

<script>
  import Banner from '../components/Banner.vue'
  import FormBurger from '../components/Form.vue'
  export default{
    name: 'Home',
    components:{
      Banner,FormBurger
    }
  }
</script>
