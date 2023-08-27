<template>
	   <h1>{{ title}}</h1>
	   <br>	
	   <br>
	   <h1>{{count}}</h1>
</template>

<script >
	 import {ref}  from 'vue'
	export default {
		  reactive:'Reactive', 
		  props:{
		  	  title:String
		  },setup(){
		  	   const count = ref(9);
		  	   function increment(){
		  	   	  count.value++;
		  	   }

		  	   return{
		  	   	   increment, 
		  	   	   count
		  	   }
		  }
	}

</script>