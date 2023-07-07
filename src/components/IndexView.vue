<template>
	<div id="topDiv" class="DivContent">
		<div id="topDivTitle">
			<myNav></myNav>
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
		
	</div>



	<div class="DivContent" id="note">
		<div>
			<v-btn>待完善</v-btn>
		</div>
	</div>
	
	
	
	<v-footer class="bg-grey-lighten-1">
		<v-row justify="center" no-gutters>
			<v-btn v-for="item in list" :key="item" class="mx-3 footBtn" rounded="xl" variant="text">
				{{item}}
			</v-btn>
			
			
			
		</v-row>
	</v-footer>

</template>



<script>
import myNav from '../components/myNav.vue';
	
	export default{
		name:"indexView",
		components:{
			myNav
		},
		data() {
			return{
				list:["Home","链接1","test3","Services","Blog","Connection"]
			}
		}
	}
</script>


<style scoped>
	@import url("../css/indexView.css");
</style>