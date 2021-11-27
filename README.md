# 1.0.0
插件市场<https://ext.dcloud.net.cn/plugin?id=2435>
## uniapp,添加我的小程序,支持自定义 custom

#### props 值说明

|    属性    | 默认值                                           |       可选       |  类型   |               简介                |
| :--------: | :----------------------------------------------- | :--------------: | :-----: | :-------------------------------: |
|  isCustom  | false                                            |     Boolean      | Boolean | 是否配置了 navigationStyle:custom |
| closeColor | true                                             |     Boolean      | Boolean |  close 按钮颜色，黑白,不用就清理  |
|  bgColor   | #E6F0FF                                          |      自定义      | String  |             背景颜色              |
|  borderR   | 5                                                |      自定义      | Number  |             圆角大小              |
|   delay    | 2000                                             |      自定义      | Number  |           延时出现时间            |
|    isAm    | true                                             |     Boolean      | Boolean |             动画效果              |
|    text    | 添加我的小程序                                   |      自定义      | String  |             提示文本              |
|  fontObj   | {color: "202020",fontSize:13px fontWeight: "0",} | 传入对应格式对象 | Object  |          提示文本 style           |


用到了 scss 插件

只显示一次 ,调试下面 

```javascript
//115 if (uni.getStorageSync("my_tips_2020")) return;
//121 this.timeOut();
```
