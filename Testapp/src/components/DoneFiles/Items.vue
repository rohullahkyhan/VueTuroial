<template>
	  <div class="main">
	  	    <h1 v-bind:class="{display:show}">Obejct Class binding of Products </h1>
	  	    <hr>

	  	     <h1 v-bind:class="[className?null:null,borderbox , hoverbox,show]">Array Class binding of Products </h1>
	  	    <hr>
             
	  </div>
</template>

<script>
	
	export default { 

        items:'Items',
        data(){

        	  return {
        	  	   
        	  	    className:"display", 
        	  	    borderbox:'box',
        	  	    hoverbox:'hoverbox',
        	  	    show:true, 
        	  	    checkdisplay:true
        	  }
        }
      
        }

</script>

<style>
	 
	 .display {
	 	  color:red;
	 }
   .box {
   	  color : #fff;
   	  background:black;
   	  transition:all 1s ease;
   }
   .hoverbox:hover{
       color:orange;

   }
</style>