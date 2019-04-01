### body
网页上显示的内容要放在body标签里
```
<body>内容</body>
```
### p
段落文本
```
<p>这是一个段落</p>
```
### hx
文章标题 h1-h6
```
<h1>一级标题</h1>
<h6>六级标题</h6>
```
### em
em表示强调
```
<em>强调斜体</em>
```
### strong 
表示更强烈的强调
```
<strong>更强烈的强调</strong>
```
### span
span标签没有语义，可为内容设置单独的样式。
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style>
        span{
            color: brown
        }
    </style>
</head>
<body>
    <p>段落一<span>titi</span></p>
    <p>段落二<span>titi</span></p>
</body>
</html>
```
### q
短文本引用
```
<q>短文本引用</q>
```
### blockquote
```
<blockquote>长文本引用</blockquote>
```
### br
```
<p>
    我是第一行<br>我想换一行
</p>
```