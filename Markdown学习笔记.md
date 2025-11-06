# 标题语法

- #### 一个#代表最大的级别，#越多表示字体越小共有六个等级

- #### 且#后要有空格才能完成字体的切换

- #### 当然在typora中字体切换较为方便，只需ctrl+相应的数字，即可切换字体大小

# 强调语法

- #### 在typora中粗体为ctrl+B，斜体为ctrl+I，下划线为ctrl+U

- #### \*为斜体，\*\*为粗体， \*\*\*斜体加粗体

- #### [Markdown 强调语法](https://markdown.com.cn/basic-syntax/emphasis.html)

# 引用语法

- #### 引用时注意，打>的时候要是<u>初始字体大小</u>不然无法引用

#### >大字体就不行

- #### 为何要强调这个一点，因为在typora中切换字体一般使用ctrl+相应的数字，就可能先入为主的将字体大小改变导致无法引用

- #### 可以嵌套引用

- #### [Markdown 引用语法 ](https://markdown.com.cn/basic-syntax/blockquotes.html)

# 列表语法

- #### 如果想要在列表中镶嵌另一种元素时需要缩进四个空格或者一个制表符（tab）<img width="1082" height="1045" alt="屏幕截图 2025-11-04 202803" src="https://github.com/user-attachments/assets/b0bea1ca-d544-4131-8f22-9cc6694cfc92" />


- #### 代码块被放在列表里时需要缩进八个空格或两个制表符（tab）

- #### [Markdown 列表语法 ](https://markdown.com.cn/basic-syntax/lists.html)

# 代码语法

- #### 要将单词或短语表示为代码，请将其包裹在反引号('')中

- #### 要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符

- #### 如果代码行数较多则可以用围栏代码块<img width="1064" height="1094" alt="屏幕截图 2025-11-04 203934" src="https://github.com/user-attachments/assets/8a584004-59dc-49a5-b70d-eafdeeffd72e" />


- #### 如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(``)中<img width="1051" height="339" alt="屏幕截图 2025-11-04 204033" src="https://github.com/user-attachments/assets/42fdaf2d-11c5-48cc-a859-d3e9463c1fbe" />


- #### [Markdown 代码语法 ](https://markdown.com.cn/basic-syntax/code.html)

# 分隔线语法

- #### 要创建分隔线，请在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容

- #### 分隔线效果如下

***

- #### 注意分隔线上下均要又空白回车<img width="1038" height="548" alt="屏幕截图 2025-11-04 204522" src="https://github.com/user-attachments/assets/1bf870f2-73ed-4471-84b8-38179fa7d66d" />


# 链接语法

- #### 超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

- #### 链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔

- #### 如[Markdown语法](https://markdown.com.cn "最好用的教程")

- #### 使用尖括号可以很方便地把URL或者email地址变成可点击的链接<https://markdown.com.cn/>

- #### 强调链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号
<img width="1084" height="634" alt="屏幕截图 2025-11-04 210444" src="https://github.com/user-attachments/assets/d5ceda06-8736-4739-b3dd-9f70490b0614" />

# 图片语法

- #### 与我而言我喜欢直接将图片拖到编译器上

- #### 给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中
<img width="1412" height="112" alt="屏幕截图 2025-11-05 090626" src="https://github.com/user-attachments/assets/ea61de67-306e-422a-8e51-ae235b7d0941" />

![shiprock c3b9a023](https://github.com/user-attachments/assets/dd6c2524-cb4e-41bc-b2c1-175d8ca4237a)

- #### 同样的图片也可以加Title，与链接的方式一致
# 转义字符语法

- #### 如果想打出一些特殊符号，可以在符号前加\

# 内嵌HTML标签

- #### HTML 的行级內联标签如 `<span>`、`<cite>`、`<del>` 不受限制，可以在 Markdown 的段落、列表或是标题里任意使用

- #### 区块元素──比如 `<div>`、`<table>`、`<pre>`、`<p>` 等标签，必须在前后加上空行，以便于内容区分<img width="1072" height="722" alt="屏幕截图 2025-11-06 083137" src="https://github.com/user-attachments/assets/ed6b733f-7acc-4210-bb5c-5ae18160b6ce" />



- #### 在 HTML 块级标签内不能使用 Markdown 语法。例如 `<p>italic and **bold**</p>` 将不起作用

# 表格

## 表格

- #### 要添加表，请使用三个或多个连字符（`---`）创建每列的标题，并使用管道（`|`）分隔每列。您可以选择在表的任一端添加管道
<img width="576" height="241" alt="屏幕截图 2025-11-06 080858" src="https://github.com/user-attachments/assets/ff4a63b0-60a6-4bab-bb24-a3b3e2377001" />

- #### 单元格宽度可以变化，如下所示。呈现的输出将看起来相同<img width="811" height="234" alt="屏幕截图 2025-11-06 080913" src="https://github.com/user-attachments/assets/c3c986b7-e8f4-44e5-a849-7775df147602" />

## 对齐

#### 您可以通过在标题行中的连字符的左侧，右侧或两侧添加冒号（`:`），将列中的文本对齐到左侧，右侧或中心
<img width="504" height="264" alt="屏幕截图 2025-11-06 081119" src="https://github.com/user-attachments/assets/dffa0318-4767-4af5-b023-fabacd3b71e2" />


 


