<template>
	  <div>
	  	  <h1>{{message}}</h1>
	  </div>
</template>

<script>
   
	export default{
		  homebind:'HomeBind', 
		  props:{
		  	 message:String
		  }
		 
		 
	}
</script>

<style type="text/css" media="screen">
	  h1 {
	  	 color:#fff;
	  }
</style>