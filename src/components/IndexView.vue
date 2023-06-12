<template>
	<div id="topDiv" class="DivContent">
		<my-nav></my-nav>
		<div id="topDivTitle">
			<h1>DYD</h1>
			<span></span>
			<span>test</span>
		</div>
	</div>
	
	<div class="DivContent">
		<span>test</span>
		
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
		background-image: url("/src/assets/topBack.png");
	}
	
	.BigText{
		font-size: 80px;
	}
	
	.DivContent{
		width: 100%;
		height: 100%;
		text-align: center;
		background-size: cover;
	}
	
	#topDivTitle{
		top: 0;
		bottom: 0;
		left: 0;
		right: 0;
		position: absolute;
		margin: auto;
	}
</style>