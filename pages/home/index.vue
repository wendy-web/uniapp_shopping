<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<view class="">
				<text class="title">{{title}}</text>
			</view>
		</view>
		<view>
			<button @click="clickHandle">go to center</button>
			<button @click="clickHandle2">go to center</button>
			<text selectable space="nbsp">text   sdefef的标签</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'home'
			}
		},
		onLoad(option) {
			// 获取到当前的页面信息
			console.log(getCurrentPages(),'getCurrentPage')
		},
		onShow() {
			console.log('onShow')
		},
		methods: {
			clickHandle() {
				console.log('333');
				uni.navigateTo({
					url: '/pages/detail/detail?name=2'
				})
			},
			// 分包的处理使用
			clickHandle2() {
				uni.navigateTo({
					url: '/subpages/news/news'
				})
			}

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
