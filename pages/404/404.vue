<template>
	<view>
		页面不存在---
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		onShow() {
			const timer = setTimeout(function() {
				clearTimeout(timer);
				// tabBar的跳转要使用switchTab使用
				uni.switchTab({
					url: '/pages/home/index'
				});
			}, 2000);
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
