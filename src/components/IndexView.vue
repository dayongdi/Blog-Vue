<template>
	<div class="contain">
		<div class="bigTitle">DYD</div>
		
		
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