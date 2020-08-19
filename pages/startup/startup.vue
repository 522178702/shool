<template>
	<view class="startup-bg">
		<view class="tips-time">
			{{time}} s
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				time:3,
				
			};
		},
		onLoad() {
			this.startTime();
		},
		methods:{
			startTime(){
				setTimeout(()=>{
					if(this.time>0){
						this.time =this.time-1;
						this.startTime();
					}else{
						uni.switchTab({
							url:"../index/index"
						})
					}
				},1000)
			}
		}
	}
</script>

<style lang="less">
	uni-page-body, uni-page-refresh{
		height: 100% !important;
	}
	.startup-bg{
		width: 100%;
		height: 100%;
		background: url(../../static/startup.png) no-repeat center;
		background-size: cover;
		position: relative;
		.tips-time{
			position: absolute;
			right: 20rpx;
			top: 20rpx;
			padding: 2rpx 30rpx;
			border-radius: 25rpx;
			color: #fff;
			background-color: rgba(0,0,0,0.1);
		}
	}
</style>
