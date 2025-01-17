# Hello-world

MARKDOWN 语法介绍
==========

# Maekdown 段落
要创建段落，请使用空白行将一行或多行文本进行分隔

# Markdown 换行语法
在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行    

## 换行（Line Break）用法的最佳实践
几乎每个 Markdown 应用程序都支持**两个或多个空格**进行换行，称为 结尾**空格（trailing  whitespace)** 的方式，但这是有争议的，因为很难在编辑器中直接看到空格，并且很多人在每个句子后面都会有意或无意地添加两个空格。
由于这个原因，你可能要使用除结尾空格以外的其它方式来换行。
幸运的是，几乎每个 Markdown 应用程序都支持另一种换行方式：HTML 的 <br> 标签。
为了兼容性，请在行尾添加“结尾空格”或 HTML 的 <br> 标签来实现换行

# Markdown 强调语法
## 粗体（Bold）
要加粗文本，请在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）
 应用程序在如何处理单词或短语中间的下划线上并不一致。为兼容考虑，在单词或短语中间部分加粗的话，请使用**星号**（asterisks) **

## 斜体（Italic）
- 要用斜体显示文本，请在单词或短语前后添加*一个星号（asterisk）或下划线（underscore）*。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格.

## 粗体（Bold）和斜体（Italic）
- 要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加***三个星号或下划线***。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。

# Markdown 引用语法
## 创建 【块】 引用
- 要创建块引用，请在段落前添加**一个 > 符号**。
> ##### for example:
>> **Dorothy followed her through many of the beautiful rooms in her castle.**
## 多个段落的块引用
- **块引用可以包含多个段落。为段落之间的空白行添加一个 > 符号**
> ##### for example:
>> Dorothy followed her through many of the beautiful rooms in her castle.
>>
>> The Witch bade her clean the pots 和 kettles 和 sweep the floor 和 keep the fire fed with wood.
## 嵌套块引用
- 块引用可以嵌套。在要**嵌套的段落前添加一个 >> 符号**
> ##### for example:
>> Dorothy followed her through many of the beautiful rooms in her castle.
>>
>>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
## 带有其它元素的块引用
- 块引用可以包含其他 Markdown 格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。
> ##### for example:
>> #### The quarterly results look great!
>>
>> - Revenue was off the chart.
>> - Profits were higher than ever.
>>
>>  *Everything* is going according to **plan**.

# Markdown 列表语法
## 有序列表
要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

## 无序列表
要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。

## 在列表中嵌套其他元素
要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：
> 段落
>> *   This is the first list item.
>> *   Here's the second list item.
>> 
>>      I need to add another paragraph below the second list item.
>>
>> *   And here's the third list item.

> 引用块
>> *   This is the first list item.
>> *   Here's the second list item.
>> 
    > A blockquote would look great below the second list item.
>> 
>> *   And here's the third list item.

> 代码块
>> 代码块通常采用**四个空格或一个制表符缩进**。当它们被**放在列表中**时，请将它们**缩进八个空格或两个制表符**
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.
> 图片
1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3.  Close the file.

> 列表
You can nest an unordered list in an ordered list, or vice versa.

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

# Markdown 代码语法
要将单词或短语表示为代码，请将其包裹在[反引号 (`) 中]，其实就是[**单引号**]
> for example:
>> At the comm和 prompt, type **'nano'**
>> 

# 转义反引号
如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(``)中，等同于 [**双引号**]

# 代码块
 要创建代码块，请将代码块的**每一行缩进至少四个空格或一个制表符**。
 >- cmd
  >>* head file
  >>* second file
  >>* third file
 >- end to

# Markdown 分隔线语法
要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。
***
---
__________

# Markdown 链接语法
链接文本放在**中括号内**，**链接地址**放在后面的**括号中**，链接title可选。
超链接Markdown语法代码：[超链接显示名](超链接地址 "超链接title")
对应的HTML代码：<a href="超链接地址" title="超链接title">超链接显示名</a>

> 超链接Markdown语法代码：[超链接显示名](超链接地址 "超链接title")
>> 超链接Markdown语法代码：[Markdown语法](https://markdown.com.cn "最棒的markdown教程")

## 给链接增加 Title
链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。
> for example:
>> 这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")

# 网址和Email地址
使用**尖括号**可以很方便地把URL或者email地址变成可点击的链接。
> for example
- <https://markdown.com.cn>
- <fake@example.com>

# 带格式化的链接
强调 **链接**, 在链接语法前后**增加星号**。 要将**链接表示为代码**，请在**方括号中添加反引号**。
>for example:
- I love supporting the **[EFF](https://eff.org)**.
- This is the *['Markdown Guide'](https://www.markdownguide.org)*.
- See the section on *['code'](#code)*.

# 引用类型链接
引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。参考样式链接分为两部分：**与文本保持内联的部分以及存储在文件中其他位置的部分**，以使文本易于阅读

## 链接的第一部分格式
- 引用类型的链接的第一部分使用**两组括号进行格式设置**。第一组方括号包围**应显示为链接的文本**。第二组括号显示了一个标签，该标签用于**指向您存储在文档其他位置的链接**。
- 尽管不是必需的，可以在**第一组和第二组括号之间包含一个空格**。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。
- for example :
- [CSDN] [https://www.csdn.net/]

## 链接的第二部分格式
- 引用类型链接的第二部分使用以下属性设置格式：
- 放在括号中的标签，其后**紧跟一个冒号和至少一个空格**（例如[label]:）。
- 链接的URL，可以选择将其括在尖括号中。
- 链接的可**选标题**，可以将其**括在双引号，单引号或括号中**。
- for example:
- [资源说明] <https://www.ncnynl.com/resources.html> 'ROS 资源说明'
- [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
- [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
- [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
- [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
- [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
- [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
- [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles) 

# Markdown 图片语法
要添加图像，请使用**感叹号 (!)**, 然后在**方括号里增加替代文本**，**图片链接放在圆括号里**，括号里的链接后可以**增加一个可选的图片标题文本**。

插入图片Markdown语法代码：**![图片alt](图片链接 "图片title")**。

对应的HTML代码：<img src="图片链接" alt="图片alt" title="图片title">

- for example:
- ![风景图片](https://www.bing.com/images/search?q=%E5%9B%BE%E7%89%87&form=IQFRBA&id=083697FD7E6F8230C39C502FFE221C16162084F7&first=1&disoverlay=1 "一棵绿色的树")

## 链接图片
给图片增加链接，请将**图像**的Markdown **括在方括号中**，然后将**链接添加在圆括号中**。
-for example:
- [![沙漠中的岩石图片](/assets/img/shiprock.jpg "Shiprock")](https://markdown.com.cn)

# Markdown 转义字符语法
要显示原本用于格式化 Markdown 文档的字符，请在**字符前面添加反斜杠字符** \

- * Without the backslash, this would be a bullet in an unordered list.
- \* Without the backslash, this would be a bullet in an unordered list.

## 特殊字符自动转义
在 HTML 文件中，有两个字符需要特殊处理： < 和 & 。 < 符号用于起始标签，& 符号则用于标记 HTML 实体，如果你只是想要使用这些符号，你必须要使用实体的形式，像是 &lt; 和 &amp;。

**&符号**其实很容易让写作网页文件的人感到困扰，如果你要打「AT&T」 ，你必须要**写成「AT&amp;T」** ，还得转换网址内的 & 符号，如果你要链接到：

- http://images.google.com/images?num=30&q=larry+bird
- 你必须要把网址转成：

- http://images.google.com/images?num=30&amp;q=larry+bird



























































