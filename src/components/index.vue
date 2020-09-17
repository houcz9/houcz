<template>
	<div class="index">
		<div class="f-full content content-default" ref="content">
			<div class="corner-text">UI/UX Design</div>
			<div class="main-text">
				<p>HOUCZ9-</p>
				<p>DESIGN WORKS <strong>作品集</strong></p>
				<div class="author-wrap">
					<p class="text">侯春智  设计</p>
					<div class="website flex">
						<a href="https://www.zcool.com.cn/u/668029" target="_blank"  title="站酷上的作品"><i class="icon-zcool"></i></a>
						<a href="https://i.ui.cn/ucenter/891224.html" target="_blank"  title="UI中国上的作品"><i class="icon-ui"></i></a>
						<a href="https://dribbble.com/houcz9" target="_blank"  title="Dribbble上的作品"><i class="icon-dribbble"></i></a>
					</div>
				</div>
			</div>
			<div class="corner-mouse"></div>
			<div class="corner-right"></div>
			<img src="../assets/images/img-4.png" @load="handleLoad" style="display: none;">
			<img src="../assets/images/img-3.png" @load="handleLoad" style="display: none;">
		</div>
		
	</div>
</template>

<script>
	export default {
		name: 'index',
		data() {
			return {
				number:0
			}
		},
		created() {
		},
		mounted(){
			this.number=0;
		},
		methods:{
			handleLoad(){
				this.number++;
				if(this.number>1){
					this.$refs.content.classList.remove("content-default");
					this.$refs.content.classList.add("content-animation");
				}
			}
		}
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>