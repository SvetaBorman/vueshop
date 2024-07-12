<template>
	<div class="card">
		<img :src="require('@/assets/img/'+dat.img)">
		<h1>{{dat.name}}</h1>
		<h1>{{dat.price}}</h1>
		<button @click="$emit('detail',dat)">О товаре</button>
	</div>

</template>

<script>
	export default{
		props:["dat"]
	}
</script>

<style>
 .card{
	border: 1px solid;
	
}

.card img{
	height: 150px;
	width: 180px;
}
</style>




