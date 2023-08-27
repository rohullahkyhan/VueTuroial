<template>
	  <div class="main">
	  	   <h1 >
	  	   	   {{msg}}
	  	   </h1>
	  	   <hr>
	  	   <p v-if="show">
	  	   	{{title}}
	  	   </p>

	  	   <p v-else>
	  	   	  He , in else side 
	  	   </p>

	  	   <button type="button" v-on:click="handel">Message</button>
	  	  
	  </div>
</template>

<script>


	
	export default {
		   name:'Home',
		   props:{
		   	   title:String, 
		   	   msg:String,

		     },data(){
		   	     return{
		   	     	show:false
		   	     }
		   },methods:{
                    handel(){
                    	 if(this.show == true){
                    	 	  this.show = true
                    	 }else {
                    	 	  this.show = false
                    	 }

                    	 this.show = !this.show
                    	  
                    }
		   }
	}

</script>


<style type="text/css" media="screen">
	  
	  .main{

	  	       width:500px;
	  	       height:200px;
	  	       background:#fff;
	  	       color:black;
	  	       padding:0px 10px;
	  	       border-radius:10px;
	  }
	  button {
	  	
	  	  padding : 5px 20px;
	  	  color:#fff;
	  	  background:black;
	  	  courser:pointer;

	  }

</style>