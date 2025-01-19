## HTML

基本构成

```html
<!DOCTYPE html>
<html lang="zh-Hans">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML-CSS-练习室</title>
</head>
<body>
    <h1>HTML-CSS-练习室</h1>
    <h2 style="color:red">古法手作网页，无任何 ai 成分，可放心食用！</h2>
    <p><strong>古法手作 HTML 网站，你值得拥有</strong></p>
    <p><em>了解更多</em></p>
    <a href="https://www.baidu.com">baidu</a>

    <ol>
        <li>第一点</li>
        <li>第二点</li>
        <li>第三点</li>
    </ol>

    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Feature</a></li>
        <li><a href="#">Menu</a></li>
    </ul>

    <blockquote>书山有路勤为径<br>学海无涯苦作舟</blockquote>

    <img src="大宅门.jpeg" alt="大宅门">
</body>
</html>
```

### 常用标签

<head> 中的内容不会展示在网页中

<body> 中的内容才会在网页中展示

<heading> 和 <p> 的内容占据一行，叫区块元素

<strong> 和 <em> （粗体和斜体）叫作行内元素

<a> 标签，与其他网页建立链接

<ol> + <li> 构成清单，会在列表前添加数字序号

<ul> + <li> 常用来构建 navbar，会在列表前添加 . 

如图所示

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/fd7ed962-188c-4a3f-9305-e05c79100c11/7cf96e79-0133-4f31-937f-edfbf4a06e4f/image.png)

<blockquote> 用来引入文字

<br> 用来换行

<img src=”” alt=””> 用来引入图片

<header> 包含logo等页首相关内容（通常来说 <header><nav></nav> </header>）

<nav> 用来放置导航栏

<main> 包含网页主要内容（<main><section></section></main>）

<section> 不同分类，模块的内容

<footer> 包含页尾内容，如版权声明等

## CSS

CSS 用于美化网页

## 引入 CSS 的三种方式：

1. 直接在标签中引入
    
    ```html
    <h2 style="color:red">古法手作网页，无任何 ai 成分，可放心食用！</h2>
    ```
    
    此种方式，只对特定行的标签有效，不是对所有的同名标签有效
    

1. 在 head 中指定 CSS 格式
    
    ```html
        <style>
            li {
                color: blue;
            }
        </style>
    ```
    
    此种方法会对文件中的所有同名标签生效
    
2. 单独提取一个 style.css 文件，方便对多网页网站的样式进行修改
    
    ```html
     <!-- 在 html 文件的 head 部分引入 -->
    <link rel="stylesheet" href="style.css"> 
    ```
    

## 常用的 CSS 属性

border 边框

padding 内边距（内容到边框的距离）

padding 跟一个值，则代表距四周的距离，如果想对四周做特定顺序的修改，则按照上 右 下 左的顺序
```
padding: 20px 0px 10px 15px (上 右 下 左)
padding: 20px 10px 20px (上 左右 下)
padding: 20px 10px (上下 左右)
padding: 10px （四周）
```
margin 外边距 （控制不同网页元素之间的距离）
