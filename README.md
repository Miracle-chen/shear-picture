# shear-picture
裁剪图片保存为base64,可用于头像上传

## 适用平台
pc/移动端

## 演示
[![演示地址]](https://github.com/caohoucheng/shear-picture/blob/master/shear-picture/image/1.gif)
[baidu]:http://www.baidu.com/img/bdlogo.gif "百度Logo"  

## 使用方法
#### 1.首先加载插件，需要用到的文件有shear.picture.js和shear.picture.css文件。
```
<!DOCTYPE html>
<html>
<head>
    ...
    <link rel="stylesheet" href="css/shear.picture.css">
    <script src="js/shear.picture.js"></script>
</head>
<body>
    ...
</body>
</html>
```
#### 2.HTML内容。
```
<div class="head-img">
  <!-- 显示图片的容器 -->
  <img class="my-img">
  <!-- 选择图片 -->
  <input type="file" class="selImg" accept="image/*" multiple="">
</div>
```
#### 3.调用Picture

Picture(图片最大值(M),确定后的回调,取消后的回调)

```
<script>
Picture(1,function(e){
  //点击确定后的回调函数
  console.log(e)
}, function(e) {
  //点击取消后的回调函数
  console.log(e)
})
</script>
```
