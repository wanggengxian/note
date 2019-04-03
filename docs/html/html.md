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
长文本引用
```
<blockquote>长文本引用</blockquote>
```
### br
换行
```
<p>
    我是第一行<br>我想换一行
</p>
```
### &nbsp
空格
```
<p>
    我是&nbsp;空格
</p>
```
### hr
水平横线
```
<body>
    下面是水平横线
    <hr>
    上面是水平横线
</body>
```
### address
地址信息
```
<body>
    <address>北京市朝阳区111号</address>
    <address>titi@gmail.com</address>
</body>
```
### code
插入单行代码
```
<code>
    print('单行代码')
</code>
```
### pre
插入多行代码
```
<pre>
    def hello():
        print('多行代码')
</pre>
```
### ul-li
无序标签
```
<body>
    <ul>
        <li>举头望明月</li>
        <li>低头思故乡</li>
    </ul>
</body>

```
### ol-li
有序标签
```
<body>
    <ol>
        <li>php</li>
        <li>c</li>
        <li>c++</li>
    </ol>
</body>
```
### div
划分逻辑区域
```
<body>
    <div>
        <h1>热点新闻排行</h1>
        <ol>
            <li>药王庙路井盖离奇失踪</li>
            <li>楼下王大爷捡了一盒盖中盖</li>
            <li>小区王阿姨勇夺莲花社区30米自由泳冠军</li>
        </ol>
    </div>
    <div>
        <h1>热门编程语言排行榜</h1>
        <ol>
            <li>php</li>
            <li>php</li>
            <li>php</li>
        </ol>
    </div>
</body>
```
### table
表格，在加入css样式之前是没有边框的。
> tbody 标签表格主体

> tr 表格的一行

> th 表头

> td 表格的一个单元格

> caption 表格标题用于描述表格内容

<body>
    <table>
        <tbody>
            <caption>机械键盘库存</caption>
            <tr>
                <th>名称</th>
                <th>价格</th>
                <th>库存</th>
            </tr>
            <tr>
                <td>filco</td>
                <td>1000</td>
                <td>999</td>
            </tr>
            <tr>
                <td>阿米洛</td>
                <td>2000</td>
                <td>777</td>
            </tr>
        </tbody>
    </table>
</body>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style type="text/css">
        table tr td,th{border:1px solid #000;}
    </style>
</head>
<body>
    <table>
        <tbody>
            <caption>机械键盘库存</caption>
            <tr>
                <th>名称</th>
                <th>价格</th>
                <th>库存</th>
            </tr>
            <tr>
                <td>filco</td>
                <td>1000</td>
                <td>999</td>
            </tr>
            <tr>
                <td>阿米洛</td>
                <td>2000</td>
                <td>777</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```
### a
链接到另一个页面
```
<body>
    <a href="https://www.google.com">某个不存在的网站</a>
</body>
```
默认情况下链接的网页实当前页面打开，可以设置在新的浏览器窗口打开
```
<body>
    <a href="https://www.google.com" target="_blank">某个不存在的网站</a>
</body>
```
### img
插入图片
> src 标识图像位置

> alt 图像不可见时替换的文本 

> title 图像可见时提示的文本

```
<img src="https://ss0.baidu.com/73x1bjeh1BF3odCf/it/u=772521751,490453158&fm=85" alt="我是google" title="google">
```
### form
表单
> action 输入的数据被传递到的地方

> method 数据传递的方式（post/get）

> label 为input元素定义标记，标签的for属性应当与相关元素的id属性相同

> name 为文本框命名，备后台程序使用。

> value 为文本输入框设置默认值

```
<body>
    <form action="save.php" method="POST">
        <label for="username">用户名</label>
        <input type="text" id="username" name="usr">
        <br>
        <label for="password">密码</label>
        <input type="password" id="password" name="pwd">
        <br>
        <input type="submit" value="提交">
    </form>
</body>
```
输入大段文字可以使用文本输入域
> rows 行数

> clos 列数

```
<body>
    <form action="">
        <label for="feedback">意见反馈</label>
        <textarea name="" id="feedback" cols="30" rows="10"></textarea>
    </form>
</body>
```
>type 作用如下

|type值        |作用   |
|------------- |------|
|text          |文本   |
|password      |密码   |
|radio         |单选   |
|checkbox      |复选   |
|submit        |提交   |
|reset         |重置   |

```
<body>
    <form action="">
        喜欢的颜色<br>
        <input type="radio" name="radio" value="黑色" checked="checked">黑色
        <input type="radio" name="radio" value="红色">红色
        <input type="radio" name="radio" value="蓝色">蓝色
        <br>
        喜欢的运动<br>
        <input type="checkbox" name="checkbox1" value="游泳">游泳
        <input type="checkbox" name="checkbox2" value="爬山">爬山
        <input type="checkbox" name="checkbox3" value="跳水">跳水
        <input type="checkbox" name="checkbox4" value="拳击">拳击
    </form>
</body>
```
> 下拉列表框,设置selected="selected"该选项默认就被选中。

```
<form action="">
    <select name="" id="">
        <option value="cy">抽烟</option>
        <option value="hj" selected="selected">喝酒</option>
        <option value="tt">烫头</option>
    </select>
</form>
```
> 设置multiple="multiple",下拉框多选(ctrl)

```
<form action="">
    <select name="" id="" multiple="multiple">
        <option value="cy">抽烟</option>
        <option value="hj" selected="selected">喝酒</option>
        <option value="tt">烫头</option>
    </select>
</form>
```
### label
如果点击了label标签的文本就会触发控件,标签for属性中的值要与控件的id值保持一致。

```
<body>
    <form action="">
        <label for="cj">抽烟</label>
        <input type="radio" id="cj">
    </form>
</body>
```