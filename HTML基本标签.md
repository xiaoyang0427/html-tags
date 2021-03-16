## HTML基本标签 ##

### 1. 基本标签 ###



```
<!DOCTYPE html>        //指当前是html5的版本来显示页面的，必须写在整个页面的第一行，它是文档                          类型的声明标签
<html lang="en">    //ang就是语言，en就是english英语，用来定义当前文档显示的语言。
<head>              // 头部标签
    <meta charset="UTF-8">  // charset是字符集，用来存储各种文字。在<head>标签内，可以通                               过<meta>标签的charset属性来规定HTML文档应该使用哪种编码。
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>第一个页面</title>  //页面的标题
</head>    
<body>   
           写代码是一件快乐的事情
</body>
</html>
```

在浏览器中打开后，如下图所示：

![](C:\Users\ACER\Desktop\基础标签.png)

### 2. 文本类标签

#### 2.1标题标签

代码中的h1，h2，h3，h4，h5，h6就是一级标题，二级标题，以此列推。

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>标题标签</h1>
    <h1>标题一共六级选</h1>
    <h2>文字加粗一行显</h2>
    <h3>由大到小依次减</h3>
    <h4>从重到轻随之变</h4>
    <h5>语法规范书写后</h5>
    <h6>具体效果刷新见</h6>
</body>
</html>
```

代码中的h1，h2，h3，h4，h5，h6就是一级标题，二级标题，以此列推。

在浏览器中打开后，如下图所示：

![](C:\Users\ACER\Desktop\标题标签.png)

#### 2.2. 段落标签和换行标签 

| 标签              | 标签语义                     | 特点                 |
| ----------------- | ---------------------------- | -------------------- |
| 段落标签：<p></p> | 可以把HTML文档分割成若干段落 | 段落与段落之间有空隙 |
| 换行标签：<br/>   | 将HTML文档强行换行           | 换行后不会有空隙     |

 ```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>体育新闻</title>
</head>
<body>
    <h1>水花61分尹达拉致胜抢断 西决勇士再胜开拓者总分2-0</h1>水花61分尹达拉致胜抢断 西决勇士再胜开拓者总分2-0

    <h4>数据统计：水花兄弟合砍61分</h4>数据统计：水花兄弟合砍61分

   <p>库里22投11中，三分14投4中，罚球11罚全中得到37分8篮板8助攻，职业生涯季后赛得分30+次数来到35次，超过哈登
    现役第三位，仅次于詹姆斯和杜兰特。</p> 

    <h4>兄弟对决升级：小库里给哥哥造成压力</h4>

    <p>库里兄弟是NBA历史上第一对在分区决赛相遇的兄弟。在西决第一场中，小库里没有给哥哥造成压力，他出场19分钟，7
    投1中只得到3分3篮板2助攻，在场期间输掉10分。</p>
    <p>作者：肖洋<br />
        2021-3-11</p>
</body>
</html>
 ```

在浏览器中打开后，如下图所示：

![](C:\Users\ACER\Desktop\换行标签.png)

#### 2.3. 文本格式化标签 ###

| 标签                           | 语义   | 备注                         |
| ------------------------------ | ------ | ---------------------------- |
| <ins></ins>  or  <u></u>       | 下划线 | <ins></ins> 语义更强烈       |
| <strong></strong>  or  <b></b> | 加粗   | <strong></strong> 语义更强烈 |
| <em></em>  or  <i></i>         | 倾斜   | <em></em>  语义更强烈        |
| <del></del>  or  <s></s>       | 删除线 | <del></del> 语义更强烈       |

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>文本格式化标签</title>
</head>
<body>
    <ins>下划线标签<br/></ins>
    <strong>加粗标签<br/></strong>
    <em>倾斜标签<br/></em>
    <del>删除线标签<br/></del>
</body>
</html>
```

![](C:\Users\ACER\Desktop\实例图像\格式化标签.png)

#### 6. <div> and <span> 标签

 <div>和<span>是没有语义的，它们是一个盒子，用来装内容

特点：1.<div>相当于一个超大盒子，独占一行

​            2.<span>相当于一个小盒子，一行可以放很多个

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>div和span标签</title>
</head>
<body>
    <div>div标签独占一行</div>
    <div>div标签独占一行</div>
    <span>span</span>
    <span>标签</span>
    <span>vscode</span>
</body>
</html>
```

在浏览器中打开后，如下图时所：

![](C:\Users\ACER\Desktop\实例图像\div和span标签.png)

### 3. 图像标签

<img,src="图像URL"/>,这是图像标签，是一个单标签，其中src是图像标签的必须属性

图像标签的其他属性：

| 属性   | 属性值   | 说明                                   |
| ------ | -------- | -------------------------------------- |
| src    | 图片路径 | 必须属性                               |
| alt    | 文本     | 替换文本。图像不能显示的文字           |
| title  | 文本     | 提示文本。把鼠标放到图像上，显示的文字 |
| width  | 像素     | 设置图像的宽度                         |
| height | 像素     | 设置图像的高度                         |
| border | 像素     | 设置图像的边框粗细                     |

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>图像标签</title>
</head>
<body>
    <h4>图片的使用：</h4>
    <img src="健康预测.jpg"/>
    <h4> alt 替换文本 图像不能显示的文本：</h4>
    <img src="健康预测1.jpg" alt="MIKA King"/>
    <h4> title 替换文本 鼠标放到图像上，提示的文字：</h4>
    <img src="健康预测.jpg" alt="MIKA King" title="MIKA"/>
    <h4> width 给图像设定宽度：</h4>
    <img src="健康预测.jpg" alt="MIKA King" title="MIKA" width="500"/>
    <h4> height 给图像设定高度：</h4>
    <img src="健康预测.jpg" alt="MIKA King" title="MIKA" height="100"/>
    <h4> border 给图像设定边框：</h4>
    <img src="健康预测.jpg" alt="MIKA King" title="MIKA" height="100" border="15"/>
</body>
</html>
```

##### 图像标签注意点

1.  图像标签拥有多个属性，必须在写在标签名后面。

2.  属性之间不分前后顺序，但要用空格分开。
3.  属性采取键值对的格式，属性=“属性值”。

### 4. 超链接标签

在HTML标签中，<a>标签用于定义超链接，作用是从一个页面链接到另一个页面，分为外部链接和内部链接

##### 1. 链接的语法格式

   <a href="跳转目标" target="目标窗口的弹出方式"> 文本或图像 <a/>

| 属性   | 作用                                                         |
| ------ | ------------------------------------------------------------ |
| href   | 用于指定模式链接目标的url地址，是必须属性                    |
| target | 用于指定链接页面的打开方式，其中_self为在当前窗口打开，是默认值； _blank为在新窗口中打开 |

##### 2. 链接的分类

1.外部链接：例如  <a href="http://www.qq.com" target="_blank"> 腾讯</a>
2.内部链接：例如  <a href="gongsijianjie.html" target="blank"> 公司简介</a>
3.空连接：例如    <a href="#"> 公司地址</a>
4.下载连接：如果href里面地址是一个文件或者压缩包，会下载这个文件
5.网页元素连接：在网页中的各种网页元素，如文本、图像、表格、音频、视频等

6.锚点链接：点击链接，可以快速定位到页面中的某个位置

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>超链接标签</title>
</head>
<body>
    <h4>1.外部标签</h4>
    <a href="http://www.qq.com" target="_blank"> 腾讯</a>
    <h4>内部链接</h4>
    <a href="gongsijianjie.html" target="blank"> 公司简介</a>
    <h4>3. 空连接：#</h4>
    <a href="#"> 公司地址</a>
    <h4>4.下载连接</h4>
    <a href="心世界.zip">下载文件</a>
    <h4>5. 网页元素链接</h4>
    <a href="http://baidu.com"><img src="img.jpg"/></a>
</body>
</html>
```

### 5.注释标签

<!--注释语句-->        快捷键  ：ctrl + /

### 6.表格类标签

#### 6.1表格标签

<table></table> 用于定义表格的标签

<tr></tr> 用于定义表格的行，必须嵌套在<table></table>中
<td></td>用于定义表格中的单元格，必须嵌套在<tr></tr>中
<th></th>用于定义表格的表头，使文本内容加粗居中显示
<thead></thead>  表格的头部区域，内部必须拥有<tr>标签。
<tbody></tbody> 表格是的主体区域，主要用于放数据本体。

| 属性名      | 属性值 | 描述                                           |
| ----------- | ------ | ---------------------------------------------- |
| align       | left   | 规定表格相对周围元素的对其方式                 |
| border      | 1或""  | 规定表格单元是都拥有边框，默认为“”，表示无边框 |
| cellpadding | 像素值 | 规定单元边沿与其内容之间的空白，默认1像素      |
| cellspacing | 像素值 | 规定单元格时间的空白，默认为2像素              |
| width       | 像素值 | 规定表格宽度                                   |

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <table align="center" border="1" cellpadding="20" cellspacing="0" width="500"> 
        <tr><th>姓名</th>   <th>性别</th>   <th>年龄</th></tr>   
        <tr><td>刘德华</td>   <td>男</td>   <td>56</td></tr>
        <tr><td>张学友</td>   <td>男</td>   <td>58</td></tr>
        <tr><td>郭富城</td>   <td>男</td>   <td>51</td></tr>
        <tr><td>黎明</td>   <td>男</td>   <td>57</td></tr>
    </table>
</body>
</html>
```

![](C:\Users\ACER\Desktop\实例图像\表格标签.png)

### 11.列表标签

| 标签名    | 定义       | 说明                                                 |
| --------- | ---------- | ---------------------------------------------------- |
| <ul></ul> | 无序列表   | 里面只能包含<li>，无顺序，<li>里面可以包含任意标签   |
| <ol></ol> | 有序列表   | 里面只能包含<li>，有顺序，<li>里面可以包含任意标签   |
| <dl></dl> | 自定义列表 | 里面只能包含<dt>和<dd>，<dt>和<dd>里面可以放任何标签 |

### 12.表单标签

#### 12.表单元素

<form></form>用于定义表单域，以实现用户信息的收集和传递

| 属性   | 属性值   | 作用                                               |
| ------ | -------- | -------------------------------------------------- |
| action | url地址  | 用于指定接收并处理表单数据的拂去其程序的url地址    |
| method | get/post | 用于设置表单数据的提交方式，取其值为get或post      |
| name   | 名称     | 用于指定表单的名称，以区分同一个页面中的多个表单域 |

##### 表单元素

<input> 是一个单标签，用于收集用户信息，包含一个type属性

<select> 可以用其定义下拉列表

  <textarea>用于定义多行文本输入的控件 

 ###### type属性

| 属性值    | 描述                                                         |
| --------- | ------------------------------------------------------------ |
| button    | 定义可点击按钮                                               |
| checkbox  | 定义复选框                                                   |
| file      | 定义输入字段和“浏览”按钮，供文件上传                         |
| hidden    | 定义隐藏的输入字段                                           |
| image     | 定义图像形式的提交按钮                                       |
| password  | 定义密码字段。该字段中的字符被掩码                           |
| radio     | 定义单选按钮                                                 |
| reset     | 定义重置按钮。                                               |
| submit    | 定义提交按钮                                                 |
| text      | 定义单行的输入字段，用户可在其中输入文本。默认宽度为20个字符 |
| name      | 定义input元素的名称                                          |
| value     | 规定input的值                                                |
| checked   | 规定此input元素首次加载时应当被选中                          |
| maxlength | 规定输入字段中的字符的最大长度                               |

#### 12.2 label标签

用于绑定一个表单元素，当点击<label>标签内的文本时，浏览器会自动将光标转到或者选择对应的表单元素上

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>input 表单元素</title>
</head>
<body>
    <form action="xxx.php" method="get">
        用户名：<input type="text" name="username" value="请输入用户值" maxlength="6"> <br>
        密码：<input type="password" name="psw"> <br>
        性别：男 <input type="radio" name="sex" value="男"> 女 <input type="radio" name="sex" value="女" checked="checked"> 其他 <input type="radio" name="sex" value="其他"> <br>
        爱好：吃饭 <input type="checkbox" name="hobby" value="吃饭"> 睡觉 <input type="checkbox" name="hobby" value="睡觉"  checked="checked"> 打豆豆 <input type="checkbox" name="hobby" value="打豆豆"> <br>
        <input type="submit" value="免费注册">
        <input type="reset" value="重新设置">
        <input type="botton" value="获取验证码"> <br>
        上传头像：<input type="file">
    </form>
</body>
</html>
```

在浏览器中打开后，如图所示：

![](C:\Users\ACER\Desktop\实例图像\input标签.png)