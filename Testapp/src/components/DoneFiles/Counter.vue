<template>
	    <div v-bind="objects">
		    <h4>{{title}}</h4>
		     <hr>
		    <button @click="count++">+</button>
		    <span>{{  count > 10 ? "Stop less then ten":count  }}</span>
		   <br>

		   <!-- dynamic binding  -->
        
           <button>Button</button>
           <a v-bind:href="home">HOME </a>

<!-- shorthand -->
<a :href="about"> ABOUT </a>
	    </div>

<!-- how to use form dynamic binding  -->

</template>



<script type="text/javascript">
      
         const objects = {
         	   id:'btn', 
         	   class:'main'
         }

	        export default {
	        	   counter:'Counter', 
	        	   props:{
	        	   	   title:String
	        	   }, data(){
	        	   	    return{
	        	   	    	  count:0
	        	   	    }
	        	   }
	        }
</script>



<style type="text/css" media="screen">
        .main {
        	  width:400px;
        	  height:300px;
        	  padding:10px;
        	  background:#fff;
        }
	   button {
	   	  padding:5px 20px;
	   	  color: #fff;
	   	  background:black; 
	   	  border-radius:2px;
	   }
	     #btn {
	     	  color : red;
	     }
</style>