<template>
	<div class="container-drawer" :class="{show:active}">
		<div @click="$emit('close')">X</div>
		<div class="card">
			<h1>{{product.name}}</h1>
			<h1>{{product.description}}</h1>
			<h1>{{product.price}}</h1>
		</div>
	</div>
</template>

<script>
export default {
	props:['product','active']
}
</script>

<style>
	.container-drawer{
		display: none;
		width: 300px;
		height: 365px;
		background-color: chartreuse;
		position: absolute;
	}

	.container-drawer.show{
		display: block;
	}

</style>