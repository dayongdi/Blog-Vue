<template>
	<div id="body" class="content">
		<v-app-bar>
			<v-btn icon="$vuetify" id="toolbarTitle"></v-btn>
			<v-spacer />
			<v-btn @click="scrollTop" class="d-none d-sm-flex myNavTitle">首页</v-btn>
			<v-btn @click="scrollAbout" class="d-none d-sm-flex myNavTitle">关于</v-btn>
			<v-btn @click="scrollNote" class="d-none d-sm-flex myNavTitle">日志</v-btn>
			<v-btn @click="scrollBoard" class="d-none d-sm-flex myNavTitle">未定义</v-btn>
			<v-btn class="d-flex d-sm-none" color="primary" icon="$vuetify" @click.stop="drawer = !drawer">
			</v-btn>
		</v-app-bar>

		<v-navigation-drawer v-model="drawer" location="right" temporary>
			<v-list>
				<v-list-item><v-btn @click="scrollTop" class="dialogItem">首页</v-btn></v-list-item>
				<v-list-item><v-btn @click="scrollAbout" class="dialogItem">关于</v-btn></v-list-item>
				<v-list-item><v-btn @click="scrollNote" class="dialogItem">日志</v-btn></v-list-item>
				<v-list-item><v-btn @click="scrollBoard" class="dialogItem">未定义</v-btn></v-list-item>
			</v-list>
		</v-navigation-drawer>
		<div class="bigTitle">DYD</div>
		<text class="smallTitle">/*这里是大永弟的个人空间*/</text>
	</div>


	<div id="aboutDiv" class="pageDiv content">
		<div class="text3" style="padding-top: 3.75rem;">关于我</div>
		<div class="divider">
			<v-divider :thickness="6" class="border-opacity-100 divider" color="success" />
		</div >
			
			<div style="text-align: center;">
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
				<span class="text4">dyd也就是大永弟</span>
			</div>

		</div>
		
	

<!-- 		<div id="aboutContentDiv">
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
			<div class="text4">可以是彩票店，小吃店，也可以是水果店</div>
			<div class="text4">当然这都是26岁的我蠢蠢的梦想😂</div>
		</div> -->


<!-- 	<div id="noteDiv" class="pageDiv content" style="background-color: whitesmoke;">
		<div class="marginDiv"></div>
		<div class="text3">日志</div>
		<div class="divider">
			<v-divider :thickness="6" class="border-opacity-100 divider" color="success" />
		</div>
	</div>


	<div id="bottomDiv" class="content" style="height:30%;width: 100%;">
	</div> -->


</template>



<script>
	export default {
		name: "indexView",
		components: {},
		data() {
			return {
				drawer: null,
				list: ["链接1", "链接2", "链接3"]
			}
		},
		methods: {
			scrollTop() {
				window.scrollTo({
					top: 0,
					left: 0,
					behavior: 'smooth'
				});
			},
			scrollAbout() {
				document.getElementById('aboutDiv').scrollIntoView({
					behavior: 'smooth',
					block: 'center'
				});
			},
			scrollNote() {
				document.getElementById('noteDiv').scrollIntoView({
					behavior: 'smooth',
					block: 'center'
				});
			},
			scrollBoard() {
				document.getElementById('bottomDiv').scrollIntoView({
					behavior: 'smooth',
					block: 'center'
				});
			},
			test() {}
		}
	}
</script>


<style scoped>
	@import url('../css/indexView.css');
</style>