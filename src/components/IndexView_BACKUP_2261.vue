<template>
	<div id="topDiv" class="text-center default-div">
		<my-nav></my-nav>
<<<<<<< HEAD
		<div id="topDivTitle">
			<h1>DYD</h1>
			<h2>这里是dyd的个人空间</h2>
		</div>
	</div>
	
	<div class="DivContent">
		<div class="abhoutSelf">
			<text3>关于我</text3>
		</div>
		
		<div class="divider">
			<v-divider :thickness="6" class="border-opacity-100 divider" color="success">
			</v-divider>
		</div>
		
		<div class="labelDiv">
			<v-btn class="label">98年</v-btn>	
			<v-btn class="label">机械人 </v-btn>
			<v-btn class="label">爱游戏</v-btn>
			
		</div>
		
		<div class="textDiv">
			<div class="text4">dyd也就是大永弟</div>
			<div class="text4">🏠住广东汕头</div>
			<div class="text4">喜欢舞美，爱🏊‍，更爱🎮</div>
			<div class="text4">22年毕业于广东寄宿吃饭大学</div>
			<div class="text4">目前在深圳</div>
			<div class="text4">现在想</div>
			<div class="text4">存点💰</div>
			<div class="text4">买到心爱的🏍️骑行到西藏</div>
			<div class="text4">再到新疆和内蒙看大草原吃大🍖</div>
			<div class="text4">未来想</div>
			<div class="text4">回到家乡有一家属于自己的小店</div>
			<div class="text4">可以是超市，小吃店，也可以是书店</div>
			<div class="text4">当然这都是26岁的我蠢蠢的白日梦😂</div>
		</div>
		
=======
		<div class="TopDivContext">
			<div class="BigText">iKun.</div>
			<div class="smallText">/*这里是DYD的站点*/</div>
		</div>
	</div>
	
	<div id="about" class="text-center default-div">
		<div class="aboutContntDiv">
			text
		</div>
>>>>>>> 0c16dd7e112f59a6d0ece8a2319b3672720535c4
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

<<<<<<< HEAD

<style scoped>
	@import url("../css/indexView.css");
=======
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
	
	
>>>>>>> 0c16dd7e112f59a6d0ece8a2319b3672720535c4
</style>