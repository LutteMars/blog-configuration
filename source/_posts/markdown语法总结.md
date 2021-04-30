---
title: MarkDown语法总结
date: 2017-04-13 01:59:51
tags: [脚本语言,编程,程序设计,思考总结,前端,效率]
description: 这只是一个语言描述的测试
---
生成目录：


###一 、字体 


粗体字：**粗体字**
__double underscores__
<strong>double asterisks</strong>

斜体字：_斜体字_
 *single asterisks*
<em>single asterisks</em>

<!--more-->

> 这是Blockquotes

>> 二、这是二级

>>> 三、这是三级

##水平线

水平线：

***（*  *  *）：
* * * 

- - -

-----------------------------

##虚线

浅虚线（中文：shift + -）：

————————————————————————————————————

中虚线（中文：shift + - & ----）
—————————————————————————————
----------------------------- 


重虚线(中文：shift + - + =)：
-——————————————————
===================


##四、着重表示

带有“\”的转义字符：
\*literal asterisks\*

带有下划线的二号粗体字：
##带有下划线的二号粗体字

文件类型着重表示: `*.ddd.txt`
``There is a literal backtick (`) here.``
<p><code>There is a literal backtick (`) here.</code></p>

代码文件着重表示：<kbd>tableviewController<kbd>

@(这是着重表示吗？)

`也曾醉酒鞭名马，唯恐多情累美人`



!!! note Hexo-admonition 插件使用示例 这是基于 hexo-admonition 插件渲染的一条提示信息。类型为 note，并设置了自定义标题。 提示内容开头留 4 个空格，可以有多行，最后用空行结束此标记。

!!! warning
    这是一条采用默认标题的警告信息。
    
!!! node "嵌套链接及引用块" 欢迎访问我的博客链接：[悟尘记](https://www.lixl.cn) >这里嵌套一行引用信息。
   


##五、链接

简单链接：See my [About](/about/) page for details. 

网址链接：<http://www.baidu.com>

qq号码：[11112121211](qq:11112121211)

邮箱： 网易邮箱: <livjunjie@163.com>

新浪微博： [@阳光下的向日葵](http://weibo.com/luttemars)

带有文字说明的链接：[百度](http://www.baidu.com)



插入图片：
![Alt text](/assets/img/1.jpeg)
![Alt text](/assets/img/personalimage.jpeg)


##表情：
星星表情:star:
微笑表情 :smiley: 


范围文字说明：

##引用

```latex
options space=20
tabstave notation=true key=A time=4/4
notes :q =|: (5/2.5/3.7/4) :8 7-5h6/3 ^3^ 5h6-7/5 ^3^ :q 7V/4 |
notes :8 t12p7/4 s5s3/4 :8 3s:16:5-7/5 :h p5/4
text :w, |#segno, ,|, :hd, , #tr
```

```math
\displaystyle
\left( \sum\_{k=1}^n a\_k b\_k \right)^2
\leq
\left( \sum\_{k=1}^n a\_k^2 \right)
\left( \sum\_{k=1}^n b\_k^2 \right)
```
```katex
\displaystyle
    \frac{1}{
        \Bigl(\sqrt{\phi \sqrt{5}}-\phi\Bigr) e^{
        \frac25 \pi}} = 1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {
        1+\frac{e^{-6\pi}}
        {1+\frac{e^{-8\pi}}
         {1+\cdots} }
        }
    }
```
```latex
f(x) = \int_{-\infty}^\infty
    \hat f(\xi)\,e^{2 \pi i \xi x}
    \,d\xi
```
##列表

列表1（-）：

- 第一条
- 第二条
- 第三条

列表2：
<ul>
<li>1</li>
<li>2</li>
<li>3</li>
</ul>

列表3（+）：

+ 1
+ 2
+ 3

列表4（*）：

* 1
* 2
* 3

列表5（数字.）：

1. tom
2. jerry
3. jack

##表格

简单表格：

|列1|列2|
|------|-----|
|是什么样的感觉|我不懂|
|只是一路上|我们都在沉默|
|其实我不要|太多的承诺|
|只要你能说声|爱我|


```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

以及时序图:

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```


##代码块

程序设计语言：

```python
import os
print "hello world"
```
```java
import java.io.*;
```

```swift
// Swift 语法示例
/// Swift 语法示例
enum Student {
    case Name(String)
    case Mark(Int, Int, Int)
}

var sutdDetails = Student.Name("aaa")
var studMarks   = Student.Mark(100, 90, 88)

switch studMarks {
    case .Name(let studName):
        print("名字是：\(studName)")
    case .Mark(let mark1, let mark2, let mark3):
        print("学生的成绩是：\(mark1), \(mark2), \(mark3)")
}
```

``` Dart
/// Flutter 语法示例
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return MaterialApp(debugShowCheckedModeBanner: false, home: EHomePage());
  }
}

class EHomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return Scaffold(
        appBar: AppBar(
          title: Text(
            "我的第一个Flutter程序",
            style: TextStyle(color: Colors.red),
          ),
        ),
        body: EBody());
  }
}

class EBody extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return Center(
      child: Text(
        "Hello Flutter",
        textDirection: TextDirection.ltr,
        style: TextStyle(fontSize: 30, color: Colors.orange),
      ),
    );
  }
}

```



