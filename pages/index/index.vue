<template>
	<view class="container">
		<view class="banner">
			<image class="banner-img" src="../../static/banner.png" mode=""></image>
			<view class="serach">
				<image class="serach-icon" src="../../static/icons/serach.png" mode=""></image>
				<image class="serach-icon" src="../../static/icons/max.png" mode=""></image>
				<image class="serach-icon" src="../../static/icons/messg.png" mode=""></image>
			</view>
		</view>
		<view class="nav">
			<view class="nav-list">
				<view>
					<image class="nav-icon" src="../../static/icons/new-icon.png" mode=""></image>
				</view>
				<text>最新</text>
			</view>
			<view class="nav-list">
				<view>
					<image class="nav-icon" src="../../static/icons/ctiy-icon.png" mode=""></image>
				</view>
				<text>同城</text>
			</view>
			<view class="nav-list">
				<view>
					<image class="nav-icon" src="../../static/icons/follow-icon.png" mode=""></image>
				</view>
				<text>关注</text>
			</view>
			<view class="nav-list">
				<view>
					<image class="nav-icon" src="../../static/icons/class-icon.png" mode=""></image>
				</view>
				<text>分类</text>
			</view>
			<view class="nav-list">
				<view>
					<image class="nav-icon" src="../../static/icons/more-icon.png" mode=""></image>
				</view>
				<text>更多</text>
			</view>
		</view>
		<view class="tips">
			<text>读吧最头条 资讯 | 国学大智慧</text>
			<image class="tips-icon" src="../../static/icons/play.png" mode=""></image>
			<text class="num">16000人已收听</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				href: 'https://uniapp.dcloud.io/component/README?id=uniui'
			}
		},
		methods: {

		}
	}
</script>

<style lang="less">
	page {
		background-color: #F2F2F2;
		padding: 0;
		margin: 0;
		font-size: 14rpx;
	}

	.container {
		.banner {
			position: relative;
			width: 100%;
			height: 350rpx;

			.banner-img {
				width: 100%;
				height: 100%;
			}

			.serach {
				position: absolute;
				right: 40rpx;
				top: 40rpx;

				.serach-icon {
					width: 50rpx;
					height: 50rpx;
					margin-left: 40rpx;
				}
			}
		}

		.nav {
			background-color: #FFFFFF;
			display: flex;
			align-items: center;
			justify-content: space-around;
			height: 120rpx;

			.nav-list {
				text-align: center;

				.nav-icon {
					width: 40rpx;
					height: 40rpx;
				}
			}
		}

		.tips {
			height: 100rpx;
			background-color: #FFFFFF;
			margin-top: 4rpx;
			font-size: 32rpx;
			display: flex;
			align-items: center;
			justify-content: space-around;

			.tips-icon {
				width: 40rpx;
				height: 40rpx;
			}

			.num {
				color: #525252;
				font-size: 22rpx;
			}
		}
	}
</style>
