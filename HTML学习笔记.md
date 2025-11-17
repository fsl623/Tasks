# HTML标签

#### 定义：通过一系列的`标签(也称为元素)`来定义文本，图像，链接等。HTML标签是由尖括号包围的关键字。

#### 标签通常成对出现，包括开始标签和结束标签（双标签），内容位于两个表标签之间，例如![image-20251111181117542](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251111181117542.png)

#### 除了双标签，也有单标签，例如![image-20251111181308174](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251111181308174.png)

#### 区别：单标签用于没有内容的元素，双标签用于有内容的元素

# HTML文件结构

![image-20251111181832830](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251111181832830.png)

#### HTML文件结构一般包含以下结构

1. #### 此处标亮的代码是告诉浏览器这是一个HTML文件![屏幕截图 2025-11-11 181927](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 181927.png)

2. #### 此处标量的代码时HTML文件的外壳，主要内容要包含在这个外壳中![屏幕截图 2025-11-11 181946](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 181946.png)

3. #### 此处代码其内部包含一些文件的原信息    ~~1~~![屏幕截图 2025-11-11 182011](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 182011.png)

4. #### 此处代码其内部所包含的就是显示在浏览器上的内容![屏幕截图 2025-11-11 182030](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 182030.png)

## HTML环境搭建小tips：在VScode中构建HTML环境时可以输入一个！选择只有一个！的那个选项可以直接将结构搭建好

# HTML常用文本标签

- #### 标题标签\<ha>文本\</ha>：a为阿拉伯数字从1到6，字体1最大6最小

- #### 文本标签\<p>文本\</p>：可以在此标签内强调内容,如果想改变段落字体要用到CSS   ~~1~~

- #### 强调标签：\<b>粗体\</b>；\<i>斜体\</i>；\<u>下划线\</u>；\<s>删除线\</s>

- 

- #### 表格标签：最外层用一个\<table>\</table>，\<tr>\</tr>为行，\<td>\<td>为列，\<th>\<th>为表头，还可以将\<table>\</table>改为\<table border="a">\</table>，此操作可以加上边框，a为阿拉伯数字，为边框的宽度

  ![屏幕截图 2025-11-11 191817](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 191817.png)![屏幕截图 2025-11-11 191759](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 191759.png)



- #### 列表标签：

  1. #### 无序列表：![屏幕截图 2025-11-11 190619](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 190619.png)

  2. #### 有序列表：![image-20251111190639555](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251111190639555.png)



- #### 其他标签： 

  1. #### \<br>：相当于回车![image-20251111195345013](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251111195345013.png)

  2. #### \<hr>：创建一个分隔线

# HTML属性

- #### 基本语法![屏幕截图 2025-11-11 192442](D:\OneDrive\图片\Screenshots\屏幕截图 2025-11-11 192442.png)

  #### 注意：有些属性是某个标签特有的，而有的属性是大部分标签都可以使用的

- #### 属性标签：

  1. #### \<a href="" target="">\</a>： 超链接标签 在`href=""`的`""`中放入链接就可以实现链接的跳转，而`target=""`是决定连接的打开方式

     #### _self：表示链接在当前窗口打开

     #### _blank：表示链接在新的标签页打开

  2. #### \<img src="" alt="" width="" height="">：在网页中嵌入图片 在`src=""`输入图片的链接或者路径，`alt=""`作用是，如果网页无法显示图片则会显示`""`中的的描述性文本，`width="" height=""`用于限制图片的宽度及高度

  3. #### \<div class="">\</div>：用于创建块级容器以便于组织页面的结构和布局，其中`class=""`是表示这个区块属于哪一类，`""`中规定为哪一类

     #### 还有快捷小技巧，如果像创建一个带有class属性的div，则只需输入`.+属性值`，如.nav

     #### 如果想要创建一个带id属性的div，只需输入`#+属性值(`等到学习完CSS JS再补充)  

  4. #### \<span>\</span>：用于内联样式化文本给文本的一部分应用样式或者是标记(等到学习完CSS JS再补充)

# HTML区块 - 块元素与行内元素

- #### 块元素(block)：通常用于组织和布局页面的主要结构和内容

  - #### 块元素通常会从新行开始，并占据整行的宽度，因此他们会在页面上成此案为一块独立的内容块

  - #### 可以包含其他块级元素和行内元素

- #### 行内元素()inline)：

  - #### 通常在同一行内呈现，不会独占一行

  - #### 只需要占据其内容的宽度

  - #### 行内元素不能包含块级元素，但可以包含其他行内元素

# HTML表单

#### 表单：表单是用于提交信息、收集数据和规范流程的工具，广泛应用于网站、应用程序和各种数据收集场景

#### 比如搜索框，选项之类的

- #### \<form>\</form>为表单内容的外壳

  - #### action属性：将收集到的信息提交到后端，属性值一般是后端所提供的API

- #### \<input >：

  - #### type属性：

    - #### text属性值：创建一个输入框

      <form><input type="text"></form>

    - #### radio属性值：创建圆形选择框

      <form><input type="radio"> 男 <input type="radio"> 女</form>
    
    - #### checkbox属性值：创建方形选择框
    
      <form><label>男</label><input type="checkbox"> <label>女</label><input type="checkbox"></form>
    
    - #### submit属性值：生成一个提交按钮，可以将所收集到的信息提交到相应位置
    
      #### 可以在后方加上value=""将按钮中的文字改为自己想要的文字
    
      
    
  - #### name属性：

    - #### gender属性值：让多个选择框变为单选框，此处需注意每一个选项框都要加上这个属性及属性值

    #### \<form>

    #### \<label>男\</label>

    #### \<input type="radio" name="gender"> 

    #### \<label>女\</label>

    #### \<input type="radio" name="gender">

    #### \</form> 

  - #### id属性：可以与label进行绑定，属性值是自己写，但要暴政每个input的id都不同

  - #### placeholder属性：在输入框中显示一段灰色的文字（无实体），属性值自己输入

    <form><input type="text"  placeholder="请输入文字"></form>

  - #### value属性：在输入框显示一段黑色的文字（有实体），属性值自己输入

    <form><input type="text"  value="请输入文字"></form> 

#### 此处可以在\<input >前加上\<span>\</span>添加文字，如

<form><span>Username:</span>
    <input type="text"  placeholder="请输入文字"></form>
#### 或者用\<label>\</label>来添加前缀，这个标签是input专用的

- #### \<label>\</label>：给input加前缀

  - #### for属性：把label绑定到input其属性值与input的id相同
