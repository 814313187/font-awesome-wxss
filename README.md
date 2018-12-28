# font-awesome-wxss
> Have problems in using? Create an issue in English for help!

用于微信小程序开发的[Fort-Awesome](https://fontawesome.com)图标库，将Fort-Awesome图标的字体文件转换成base64编码储存在wxss文件中，开发者可以按照调用css文件的思路直接导入font-awesome，仅支持Fort-Awesome免费图标(Brands,Solid,Regular)  

**注意：仅接受纠错类型的merge**  

## 使用方法  
在[release页面](https://github.com/McContax/font-awesome-wxss/releases)下载最新版的压缩包，解压之后的文件结构如下
```
│--LICENSE
│--README.md 
│--wxss
    │---all.min.wxss
    │---all.wxss
    │---brands.min.wxss
    │---brands.wxss
    │---fontawesome.min.wxss
    │---fontawesome.wxss
    │---regular.min.wxss
    │---regular.wxss
    │---solid.min.wxss
    │---solid.wxss
```
复制all.min.wxss到小程序项目的根目录下，在app.wxss第一行加上
```
@import "./all.min.wxss";
```
然后在wxml需要的地方加入
```
<i class="fab fa-apple"></i>
```
*********
如果觉得all文件太大了自己用不到这么多，可以仅移动自己需要的图标类型的文件，例如要导入苹果的logo，需要在app.wxss第一行插入
```
@import "./fontawesome.min.wxss";
@import "./brands.min.wxss";
```
然后在相关的wxml文件中
```
<i class="fab fa-apple"></i>
```

## 相关链接
[Fort-Awesome官网](https://fontawesome.com)  
[Fort-Awesome官方GitHub](https://github.com/FortAwesome)
