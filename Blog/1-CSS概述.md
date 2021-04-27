# CSS 概述

## 1. CSS目的

为了更好的美化网页，字体，大小，CSS选择器等等

## 2.快速入门

### 不分离版本-内部样式

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS-1</title>
</head>
    <!--用style来编写CSS代码
    语法：
        选择器{
            statement 1；
            statement 2：
            statement 3；
    -->
 
    <style>
        h1{
            color: red;
        }
    </style>
    
<body>

    <h1>我是标题一</h1>

</body>
</html>
```

style tage: 用style tage这个标签和h1标题进行关联使字体颜色变为红色

### 或者使用style直接写在tag中

```html
    <h1 style="color:green";>我是标题一</h1>
```



### 分离版本-外部链接: 推荐使用

xxx.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS-1</title>
</head>

    <link rel="stylesheet" href="style.css">

<body>

    <h1>我是标题一</h1>

</body>
</html>
```

style.css

```css
h1{
    color: red;
}
```



将css的内容写在一个style.css文件内，在html中用link tag进行关联，实现css内容和HTML内容分离便于管理