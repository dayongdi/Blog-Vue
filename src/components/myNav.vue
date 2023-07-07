<template>
	<v-app-bar>
		<v-btn icon="$vuetify" id="toolbarTitle"></v-btn>
		<v-spacer></v-spacer>
		<v-btn @click="scrollTop" class="d-none d-sm-flex myNavTitle">首页</v-btn>
		<v-btn @click="scrollAbout" class="d-none d-sm-flex myNavTitle">关于</v-btn>
		<v-btn @click="scrollNote" class="d-none d-sm-flex myNavTitle">日志</v-btn>
		<v-btn @click="scrollBoard" class="d-none d-sm-flex myNavTitle">未定义</v-btn>
		<a class="d-none d-sm-flex myNavTitle"></a>
		<v-btn
			class="d-flex d-sm-none"
            color="primary"
			icon="$vuetify"
            @click.stop="drawer = !drawer"
          >
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
	
	
	
</template>


<script>
	export default{
		name:"MyNav",
		data: () => {
			return{
				drawer:null,
			}
		},
		methods:{
			scrollTop(){
				window.scrollTo({
					top:0,
					left:0,
					behavior:'smooth'
				});
			},
			scrollAbout(){
				window.scrollTo({
					top:840,
					left:0,
					behavior:'smooth'
				});
			}
			,
			scrollNote(){
				window.scrollTo({
					top:1680,
					left:0,
					behavior:'smooth'
				});
			},
			scrollBoard(){
				window.scrollTo({
					top:2520,
					left:0,
					behavior:'smooth'
				});
			}
			
		}
	}
</script>

<style scoped>
@import url("../css/nav.css");
</style>