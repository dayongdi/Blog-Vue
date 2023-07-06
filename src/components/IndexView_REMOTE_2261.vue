<template>
	<div id="topDiv" class="text-center default-div">
		<my-nav></my-nav>
		<div class="TopDivContext">
			<div class="BigText">iKun.</div>
			<div class="smallText">/*这里是DYD的站点*/</div>
		</div>
	</div>
	
	<div id="about" class="text-center default-div">
		<div class="aboutContntDiv">
			text
		</div>
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
	.BigText{
		color: aliceblue;
		font-size: 70px;
	}
	
	.smallText{
		color: aliceblue;
		font-size: 20px
	}
	
	#topDiv{
		background-image: url("/src/assets/backgournd.png");
		background-repeat: no-repeat;
		background-size: cover;
		background-attachment: fixed;
		width: 100%;
		height: 100%;
/* 		position: fixed;
		top: 0;
		left: 0;
		right: 0;
		bottom: 0; */
	}
	
	.TopDivContext{
		position: absolute;
		top: 45%;
		width: 100%;
		height: 100%;
	}
	
	.default-div{
		height: 100%;
		max-width: 100%;
		max-height: 100%;
	}
	
	
</style>