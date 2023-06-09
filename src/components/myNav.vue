<template>
	<v-app-bar>
		<v-btn icon="$vuetify" id="toolbarTitle"></v-btn>
		<v-spacer></v-spacer>
		<div></div>
		<v-btn class="d-none d-sm-flex">首页</v-btn>
		<v-btn class="d-none d-sm-flex">关于</v-btn>
		<v-btn class="d-none d-sm-flex">日志</v-btn>
		<v-btn class="d-none d-sm-flex">留言板</v-btn>
		<v-btn class="d-none d-sm-flex">待定</v-btn>
		
		
	</v-app-bar>
	
</template>

<script>
	
	export default{
		name:"MyNav"
	}
</script>

<style>
</style>