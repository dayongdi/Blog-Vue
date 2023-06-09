<template>
	<v-app-bar>
		<v-btn icon="$vuetify" id="toolbarTitle"></v-btn>
		<v-spacer></v-spacer>
		<v-btn class="d-none d-sm-flex myNavTitle">首页</v-btn>
		<v-btn class="d-none d-sm-flex myNavTitle">关于</v-btn>
		<v-btn class="d-none d-sm-flex myNavTitle">日志</v-btn>
		<v-btn class="d-none d-sm-flex myNavTitle">留言板</v-btn>
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
			<v-list-item><v-btn class="dialogItem">首页</v-btn></v-list-item>
			<v-list-item><v-btn class="dialogItem">关于</v-btn></v-list-item>
			<v-list-item><v-btn class="dialogItem">日志</v-btn></v-list-item>
			<v-list-item><v-btn class="dialogItem">留言板</v-btn></v-list-item>
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
		}
	}
</script>

<style>
.myNavTitle{
	text-align: center;
	width: 5%;
	margin-left: 1%;
	margin-right: 1%;
}

.dialogItem{
	width: 100%;
}
</style>