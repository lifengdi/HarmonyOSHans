# HarmonyOSHans

HarmonyOS-Hans 的切片文件，可以部署到 CDN 上，为站点添加 HarmonyOS 字体支持。

## 使用方法

### 上传字体切片及CSS文件到你的网站或者其他CDN服务

创建HarmonyOSHans文件夹，将css文件以及font文件夹上传到HarmonyOSHans文件夹。

### 引入字体

```html
<link rel="stylesheet" href="https://yourdomain.com/HarmonyOSHans/common.css">
```

### 使用字体

根据需要在 CSS 中添加 `HarmonyOSHans-Regular` 字体，本例样式中已自适应字宽。

```html
<style>
  body {
    font-family: 'HarmonyOSHans-Regular', sans-serif;
  }
</style>
```

您也可以直接使用以下CSS代码：
```css
/* 字体相关css */
@import url("https://yourdomain.com/HarmonyOSHans/common.css");
@font-face {
  font-family: "HarmonyOSHans-Regular", sans-serif;
  font-weight: normal;
  font-style: normal;
}
*:not([class*="icon"]):not(i) {
  font-family: "HarmonyOSHans-Regular" !important;
}
```

> 注意：需要将https://yourdomain.com/HarmonyOSHans/common.css替换成为您自己的链接
