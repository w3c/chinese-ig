# 小程序标准化概要

## 可以标准化的部分

本节包括可以标准化的部分。

### JSON 配置

#### 全局和页面配置

此部分包括小程序的全局配置和每个页面的局部配置，如：

* 页面路径列表（全局配置）
* 底部 tab 栏样式（全局配置）
* 网络请求的超时时间（全局配置）
* debug 模式（全局配置）
* 分包结构配置（全局配置）
* 使用的权限（全局配置）
* 窗口样式（状态栏、导航条、标题、窗口背景色等，包括全局和页面配置）

相关规范：[Web App Manifest](https://www.w3.org/TR/appmanifest/)

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/tutorial/process_page/)
* [快应用](https://doc.quickapp.cn/tutorial/getting-started/project-configuration.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/framework/config.html)

### 组件

包括自带组件和自定义组件。

自定义组件相关规范：

* HTML: [template](https://html.spec.whatwg.org/multipage/scripting.html#the-template-element), [custom elements](https://html.spec.whatwg.org/multipage/custom-elements.html#custom-elements), [ES modules](https://html.spec.whatwg.org/multipage/webappapis.html#integration-with-the-javascript-module-system)
* CSS: [CSS Scoping](https://drafts.csswg.org/css-scoping/), [CSS Shadow Parts](https://drafts.csswg.org/css-shadow-parts/)
* DOM: [shadow DOM](https://dom.spec.whatwg.org/#shadow-trees)

自定义组件的现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/framework/custom-component/)
* [快应用](https://doc.quickapp.cn/tutorial/framework/parent-child-component-communication.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/framework/custom-component/)

### 蓝牙

相关规范：[Web Bluetooth](https://webbluetoothcg.github.io/web-bluetooth/)

现有实现：

* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/device/bluetooth/wx.onBLECharacteristicValueChange.html)

### NFC

相关规范：[Web NFC API](https://w3c.github.io/web-nfc/)

现有实现：

* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.stopHCE.html)

### 地理位置

相关规范：

* [Geolocation API](https://www.w3.org/TR/geolocation-API/)
* [Geolocation Sensor](https://www.w3.org/TR/geolocation-sensor/)

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/api/location_get/)
* [快应用](https://doc.quickapp.cn/features/system/geolocation.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.getLocation.html)

### 电池状态

相关规范：

* [Battery Status API](https://www.w3.org/TR/battery-status/)

现有实现：

* [快应用](https://doc.quickapp.cn/features/system/battery.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.getBatteryInfo.html)

### 加速计/罗盘/设备方向/陀螺仪

相关规范：

* [Generic Sensor](https://www.w3.org/TR/generic-sensor/)
* [Accelerometer](https://www.w3.org/TR/accelerometer/)
* [Gyroscope](https://www.w3.org/TR/gyroscope/)
* [Magnetometer](https://www.w3.org/TR/magnetometer/)
* [Orientation Sensor](https://www.w3.org/TR/orientation-sensor/)
* [Screen Orientation](https://www.w3.org/TR/screen-orientation/)
* [DeviceOrientation Event](https://w3c.github.io/deviceorientation/)

现有实现 API 数目较多，暂不列出。

### 振动

相关规范：

* [Vibration API](https://www.w3.org/TR/vibration/)

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/api/device_vibrate/)
* [快应用](https://doc.quickapp.cn/features/system/vibrator.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.vibrateShort.html)

### 剪贴板

相关规范：

* [Clipboard API and events](https://www.w3.org/TR/clipboard-apis/)
* [execCommand](https://w3c.github.io/editing/execCommand)

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/api/device_clipboard/)
* [快应用](https://doc.quickapp.cn/features/system/clipboard.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.setClipboardData.html)

### 屏幕

此部分包括设置屏幕亮度、截屏等与屏幕相关的功能。

相关规范：无

现有实现：

* [快应用](https://doc.quickapp.cn/features/system/brightness.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.setScreenBrightness.html)

### 网络信息

相关规范：

* [Network Information API](https://wicg.github.io/netinfo/)

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/api/device_network/)
* [快应用](https://doc.quickapp.cn/features/system/network.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.onNetworkStatusChange.html)

### 认证

相关规范：

* [Web Authentication](https://www.w3.org/TR/webauthn/)

现有实现：

* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.startSoterAuthentication.html)

### 本地存储

相关规范：

* HTML: [Web storage](https://html.spec.whatwg.org/multipage/webstorage.html#the-localstorage-attribute)
* [IndexedDB](https://w3c.github.io/IndexedDB/)
* [File API](https://www.w3.org/TR/FileAPI/)
* [Native File System API](https://wicg.github.io/native-filesystem/)

现有实现 API 数目较多，暂不列出。

### 网络请求

相关规范：

* [Fetch](https://fetch.spec.whatwg.org/)

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/api/net_request/)
* [快应用](https://doc.quickapp.cn/features/system/fetch.html)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.request.html)

### 图片/视频/音频

保存到本地、全屏预览、获取媒体信息、播放（暂停、倍速、弹幕、跳转到指定位置、后台播放等）

### 直播

### 录音/拍照/录像

### 支付

相关规范列表：https://w3c.github.io/web-roadmaps/mobile/payment.zh.html

现有实现 API 数目较多，暂不列出。

### 通知/推送

相关规范：

* [Notifications API](https://notifications.spec.whatwg.org/)
* [Push API](https://www.w3.org/TR/push-api/)

现有实现 API 数目较多，暂不列出。

### 拨打电话？

相关规范：无

现有实现：

* [百度智能小程序](https://smartprogram.baidu.com/docs/develop/api/device_call/)
* [微信小程序](https://developers.weixin.qq.com/miniprogram/dev/api/wx.makePhoneCall.html)

### 页面管理逻辑？

## 其他部分

本节包括标准化意义不大或者比较困难的部分。

### JSON 配置

#### 开发者工具配置

#### 模板语言

#### 流量统计和数据分析

#### MVVM 架构？

#### 二维码？

#### 地图？

#### 系统信息？

获取部分系统信息可能会有潜在的安全和隐私问题。
