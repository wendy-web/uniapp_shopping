<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		},
		// 404 页面不存在时跳转
		onPageNotFound: function() {
			uni.navigateTo({
				url: '/pages/404/404'
			});
		},
		onThemeChange: function(options) {
			console.log(':onThemeChange监听系统主题变化')
			console.log(options)
		},
	}
</script>

<style>
	/*每个页面公共css */
</style>
