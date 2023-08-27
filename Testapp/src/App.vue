<script setup>

// import TheWelcome from './components/TheWelcome.vue'
// import Home from './components/Home.vue'
// import Products from './components/Products.vue'
// import Counter from './components/Counter.vue'
// import Reactive from './components/Reactive.vue'
// import Footer from './components/Footer.vue'
// import  Items from './components/Items.vue'


import HomeBind from './components/HomeBind.vue';
import DataBind from './components/DataBind.vue';

</script>


<template>
  

  <center>
       <main>
            <HomeBind message="{message}" />
            <DataBind  />
       </main>
      
  </center>


</template>


<style type="text/css">
  
  *{
      padding: 0px;
      margin:0px;
      font-family: tahoma;
  }
  body{
      background: black;
  }

  main {
      margin-top: 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
  }

</style>






