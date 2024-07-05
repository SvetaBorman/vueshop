<template>
  <div class="home">
   <ProductCard/>
  </div>
</template>

<script>

import items from '@/data/item';
import ProductCard from "@/components/ProductCard.vue"

export default {
name: 'HomeView',
  components: {ProductCard
  },
 data(){
	return{
		items:items
	}
  }
}
</script>
