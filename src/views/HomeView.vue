<template>
  <div class="home">
	<ProductDescription
		:active='active.drawer'
		:product='product'
		v-on:close="closeDetailProduct()"
	/>

   <ProductCard 
	v-for="item in items"
	:key="item.id"
	:dat="item"
	v-on:detail="detailProduct($event)"
	/>
  </div>
</template>

<script>

import items from '@/data/item';
import ProductCard from '@/components/ProductCard.vue';
import ProductDescription from '@/components/ProductDescription.vue';

export default {
name: 'HomeView',
	components: {ProductCard,ProductDescription
	},
	data(){
		return{
			items:items,
			active:{
				drawer:false
			},
			product: 0
		}
	},
	methods:{
		detailProduct(dat){
			this.active.drawer= true;
			this.product=dat;
		},

		closeDetailProduct(){
			this.active.drawer= false;
		}
	}
}
</script>

<style>
	.home{
		display: flex;
		justify-content: space-around;
	}
</style>
