# 1.0.0

## uniapp,添加我的小程序,支持自定义 custom

close 按钮 2 个 base64 按钮比较大 可替换下～

### 使用方法

#### 引入

```javascript
import aTip from "@/components/a_tip/aTip";
Vue.component("WxTip", aTip);
```

```html
<!-- 自定义导航 -->
<aTip :isCustom="true"></aTip>
<!-- 加参数 -->
<aTip :isCustom="" :bgColor="" :text="" :fontObj="fontObj" :borderR="5" :isAm=""></aTip>
```

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

只会显示一次
用到了 scss 插件
调试注释下面 2 句

```javascript
//115 if (uni.getStorageSync("my_tips_2020")) return;
//121 this.timeOut();
```
