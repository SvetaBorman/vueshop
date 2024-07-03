<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
	 <TestBasket/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import TestBasket from "@/components/TestBasket.vue"

export default {
  name: 'HomeView',
  components: {
    HelloWorld, TestBasket
  }
}
</script>
