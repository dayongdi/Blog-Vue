<template>
	<div class="contain">
		<div class="bigTitle">DYD</div>
		<div class="smallTitile">/*这里是大永弟的个人空间*/</div>
	</div> 
	
	<div class="containDiv">
		<div id="about" class="normalTitle" >关于</div>
		<div class="divider">
			<v-divider :thickness="5" class="border-opacity-100 divider" color="success" />
		</div >
		
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
	
	<div class="containDiv_recommond">
		<div id="recommond" class="normalTitle">推荐</div>
		<div class="divider">
			<v-divider :thickness="5" class="border-opacity-100 divider" color="success" />
		</div>
			
		<v-table class="recommond_table">
			<div class="table-item"></div>
			<div class="table-item"></div>
			<div class="table-item"></div>
			<div class="table-item"></div>
			<div class="table-item"></div>
			<div class="table-item"></div>
		</v-table>
		
	</div>
	
	<div class="containDiv_bottom">
		<div id="bottom" class="normalTitle">日记</div>
		<div class="divider">
			<v-divider :thickness="5" class="border-opacity-100 divider" color="success" />
		</div >
			

	</div>
	
	

	
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