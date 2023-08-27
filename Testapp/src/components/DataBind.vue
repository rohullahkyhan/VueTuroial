<template>
	  <div>
	  	  <h1>{{message}}</h1>
	  	  <input type="text"  v-model="message">
	  </div>
</template>

<script>
	   export default{
	   	   name:'DataBind', 
	   	   data(){
	   	   	  return{
	   	   	  	  message:"Hello, Send to Child to Parent if it work "
	   	   	  }
	   	   }
	   }
</script>


<style type="text/css" media="screen">
	  h1 {
	  	color:#fff;
	  }
</style>