<template>
	<div class="contain">
		<div class="topNav">
			<v-btn icon="$vuetify"></v-btn>
			<v-spacer></v-spacer>
			<v-btn class="d-none d-sm-flex button"  @click="scrollTop" 	color="transparent">
				<div class="button_text">首页</div>
			</v-btn>
			
			<v-btn class="d-none d-sm-flex button"  @click="scrollAbout" color="transparent">	
				<div class="button_text">关于</div>
			</v-btn>
			<v-btn class="d-none d-sm-flex button"  @click="scrollRecommond" color="transparent">
				<div class="button_text">推荐</div>
			</v-btn>
			<v-btn class="d-none d-sm-flex button"  @click="scrollBoard" color="transparent">
				<div class="button_text">未定义</div>
			</v-btn>
		</div>
		<div class="bigTitle">DYD</div>

		<div class="smallTitile">/*这里是大永弟的个人空间*/</div>
		<v-btn
			class="d-flex d-sm-none drawable"
			color="primary"
			icon="$vuetify"
			@click.stop="drawer = !drawer"
		  />
	</div>	
	
	
	<div class="containDiv" @click.stop="drawer = !drawer">
		<div class="containDiv_about" id="about">
			<div class="normalTitle" >关于</div>
			<v-divider :thickness="5" class="border-opacity-100 divider" color="success" />
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
			<div class="text_content">test1.......</div>
		</div>
		
		<div class="containDiv_recommond" id="recommond" @click.stop="drawer = !drawer">
			<div class="normalTitle" >推荐</div>
			<v-divider :thickness="5" class="border-opacity-100 divider" color="success" />
			
			<div class="recommond_list">
				<div class="list-item"></div>
				<div class="list-item"></div>
				<div class="list-item"></div>
				<div class="list-item"></div>
			</div>
		</div>
		
		<div class="containDiv_bottom" id="bottom" @click.stop="drawer = !drawer">
			<div class="normalTitle" >未定义</div>
			<v-divider :thickness="5" class="border-opacity-100 divider" color="success" />
			
		</div>
	</div>
	

	


	<v-navigation-drawer v-model="drawer" location="right" temporary>
		<v-list>
			<v-list-item><v-btn @click="scrollTop" class="dialogItem">首页</v-btn></v-list-item>
			<v-list-item><v-btn @click="scrollAbout" class="dialogItem">关于</v-btn></v-list-item>
			<v-list-item><v-btn @click="scrollRecommond" class="dialogItem">日志</v-btn></v-list-item>
			<v-list-item><v-btn @click="scrollBoard" class="dialogItem">未定义</v-btn></v-list-item>
		</v-list>
	</v-navigation-drawer>

	
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
				document.getElementById('about').scrollIntoView({
					behavior: 'smooth',
					block: 'center'
				});
			},
			scrollRecommond() {
				document.getElementById('recommond').scrollIntoView({
					behavior: 'smooth',
					block: 'center'
				});
			},
			scrollBoard() {
				document.getElementById('bottom').scrollIntoView({
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