<template>
	<h1>Корзина</h1>
	<TestBasket/>
	<TestBasket/>
</template>

<script>
import TestBasket from "@/components/TestBasket.vue"

export default{
	name: "BasketView",
	components:{
		TestBasket
	}	  
}
</script>

<style>

</style>