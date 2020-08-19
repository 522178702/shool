<script>
	export default {
		onLaunch: function() {
			console.log('App Launch');
		},
		onShow: function() {
			console.log('App Show');
		},
		onHide: function() {
			console.log('App Hide');
		}
	};
</script>

<style>
	/* 解决头条小程序组件内引入字体不生效的问题 */
	/* #ifdef MP-TOUTIAO */
	@font-face {
		font-family: uniicons;
		src: url('/static/uni.ttf');
	}

	/* #endif */
	.uni-tabbar__item:nth-child(4)>.uni-tabbar__bd {
		position: absolute;
		top: -15px;
	}

	.uni-tabbar__item:nth-child(4)>.uni-tabbar__bd>.uni-tabbar__icon {
		width: 53px;
		height: 53px;
		background: #fff;
		border-top-left-radius: 50%;
		border-top-right-radius: 50%;
		border-top: 1px solid rgba(0, 0, 0, 0.33);
	}
</style>
