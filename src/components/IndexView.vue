<template>
	<div id="topDiv" class="text-center">
		<my-nav></my-nav>
		<div class="BigText">Blog</div>
		<a>/*这里是DYD的测试*/</a>
	</div>
	
</template>

<script>
import myNav from '../components/myNav.vue';
	export default{
		name:"indexView",
		components:{
			myNav
		}
	}
</script>

<style>
	#topDiv{
		height: 100%;
		max-width: auto;
		max-height: 100%;
		background-image: url("/src/assets/topBack.jpg");
	}
	
	.BigText{
		font-size: 80px;
	}
</style>