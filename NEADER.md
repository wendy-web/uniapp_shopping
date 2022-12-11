待解决的配置
#### pages.json的启动模式配置
问题：微信的小程序配置出现错误的提示，且不可运行；
```json
"condition": { //模式配置，仅开发期间生效
		"current": 0, //当前激活的模式（list 的索引项）
		"list": [
			{
				"name": "home",
				"path": "pages/home/index"
			},
			{
				"name": "我的", //模式名称
				"path": "pages/center/index" //启动页面，必选
			},
			{
				"name": "message",
				"path": "pages/message/index"
			}
		]
	}
```