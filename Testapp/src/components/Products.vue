<template>
	   <div style="color:white">
	   	     {{title}} 

	   	     <table>
	   	     	
	   	     	<thead>
	   	     		<tr>
	   	     			<th>ID</th>
	   	     			<th>NAME</th>
	   	     			<th>LASTNAME</th>
	   	     			<th>AGE</th>
	   	     		</tr>
	   	     	</thead>
	   	     	<tbody>
	   	     		<tr>
	   	     		<div v-for="item in data">
	   	     		     
	   	     		     	<td>{{item.id}}</td>
	   	     		     	<td>{{item.name}}</td>
	   	     		     	<td>{{item.lname}}</td>
	   	     		     	<td>{{item.age}}</td>
	   	     		     
	   	     		</div>
	   	     		</tr>
	   	     	</tbody>
	   	     </table>
	   </div>



</template>

<script type="text/javascript">
	

	   export default{
	   	     name:'Products', 
	   	     props:{
	   	     	 title:String
	   	     },data(){
	   	     	  return {
	   	     	  	   data:[

                           {id:1,name:'Rohullah', lname:'Kyhan' , age:'21'},
                           {id:2,name:'Mosa', lname:'Ahamdi' , age:'21'},
                           {id:3,name:'Hikmatullah', lname:'Baran' , age:'25'}
	   	     	  	   	]
	   	     	  }
	   	     }
	   }

</script>