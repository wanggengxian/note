## 样式
内联式 > 嵌入式 > 外部式
### 内联式
```
<body>
    <p style="color:red; font: size 12px;">12号红色</p>
</body>
```
### 嵌入式
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        p{
            color:blue;
            font: 13px;
        }
    </style>
</head>
<body>
    <p>13号的蓝色</p>
    <p>13号的蓝色</p>
</body>
</html>
```
### 外部式
下例中的base.css文件放在了当前目录下，rel type为固定写法不可修改。
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="base.css" type="text/css">
</head>
<body>
    <p>13号的蓝色</p>
    <p>13号的蓝色</p>
</body>
</html>
```
## 选择器
{}前面的就是选择器
```
<style>
    p{
        color: red;
    }
</style>
```
### 标签选择器
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        h1{
            color: red;
        }
    </style>
</head>
<body>
    <h1>一只红色的H1标题</h1>
</body>
</html>
```
### 类选择器
.开头
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        .tt{
            color: blue;
        }
    </style>
</head>
<body>
    <p class="tt">类选择器</p>
    <p >哈哈</p>
    <p class="tt">类选择器</p>
</body>
</html>
```
### ID选择器
\#开头
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        #nn{
            color:red;
        }
    </style>
</head>
<body>
    <p class="tt" id="nn">ID选择器</p>
    <p >哈哈</p>
    <p class="tt" id="nn">ID选择器</p>
</body>
</html>
```
### 子选择器
用于选择指定标签的子元素，作用于第一后代。
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        .nn>li{
            border: 1px solid red;
        }
    </style>
</head>
<body>
    <ul class="nn">
        <li>水果
            <ul>
                <li>香蕉</li>
                <li>苹果</li>
                <li>橘子</li>
            </ul>
        </li>
        <li>蔬菜
            <ul>
                <li>白菜</li>
                <li>萝卜</li>
                <li>面条</li>
            </ul>
        </li>
    </ul>
</body>
</html>
```
### 包含(后代)选择器 
作用与元素的所有后代
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        .nn li{
            border: 1px solid red;
        }
    </style>
</head>
<body>
    <ul class="nn">
        <li>水果
            <ul>
                <li>香蕉</li>
                <li>苹果</li>
                <li>橘子</li>
            </ul>
        </li>
        <li>蔬菜
            <ul>
                <li>白菜</li>
                <li>萝卜</li>
                <li>面条</li>
            </ul>
        </li>
    </ul>
</body>
</html>
```
### 通用选择器
匹配HTML中所有的标签元素
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        *{
            color: red;
        }
    </style>
</head>
<body>
    <h1>举头望明月</h1>
    <h2>低头思故乡</h2>
    <p>锄禾日当午</p>
    <ul class="nn">
        <li>水果
            <ul>
                <li>香蕉</li>
                <li>苹果</li>
                <li>橘子</li>
            </ul>
        </li>
        <li>蔬菜
            <ul>
                <li>白菜</li>
                <li>萝卜</li>
                <li>面条</li>
            </ul>
        </li>
    </ul>
</body>
</html>
```
### 伪类选择符
允许给html不存在的标签设置样式,鼠标滑过 谷歌 会变成红色。
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        a:hover{
            color: red;
        }
    </style>
</head>
<body>
    <p>
        有事找<a href="www.google.com">谷歌</a>
    </p>
</body>
</html>
```
### 分组选择器
对标签元素分组后，可为同组内的不同标签元素设置相同的样式。
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        .tt,#nn span{
            color: red;
        }
    </style>
</head>
<body>
    <p class="tt">
        举头望明月<span>低头思故乡</span>
        <h1>奥特曼</h1>
    </p>
    <p id="nn">
        锄禾日当午<span>汗滴禾下土</span>
    </p>
</body>
</html>
```