# HTML标签

#### 定义：通过一系列的`标签(也称为元素)`来定义文本，图像，链接等。HTML标签是由尖括号包围的关键字。

#### 标签通常成对出现，包括开始标签和结束标签（双标签），内容位于两个表标签之间，例如<img width="715" height="158" alt="屏幕截图 2025-11-11 181114" src="https://github.com/user-attachments/assets/1cce14bf-310e-4560-8c62-874e4ccb161f" />

#### 除了双标签，也有单标签，例如<img width="834" height="179" alt="屏幕截图 2025-11-11 181303" src="https://github.com/user-attachments/assets/697e9928-573b-44a5-a3e7-f9df3bfe0bb6" />

#### 区别：单标签用于没有内容的元素，双标签用于有内容的元素

# HTML文件结构

<img width="1189" height="910" alt="屏幕截图 2025-11-11 181758" src="https://github.com/user-attachments/assets/7c611621-00e7-4580-b119-d1fc32616072" />


#### HTML文件结构一般包含以下结构

1. #### 此处标亮的代码是告诉浏览器这是一个HTML文件<img width="1195" height="914" alt="屏幕截图 2025-11-11 181927" src="https://github.com/user-attachments/assets/4c7f1ceb-0b8b-421a-8936-82b30325a517" />


2. #### 此处标量的代码时HTML文件的外壳，主要内容要包含在这个外壳中<img width="1177" height="900" alt="屏幕截图 2025-11-11 181946" src="https://github.com/user-attachments/assets/569cb325-fde4-4227-af66-c436f3873126" />


3. #### 此处代码其内部包含一些文件的原信息 <img width="1167" height="899" alt="屏幕截图 2025-11-11 182011" src="https://github.com/user-attachments/assets/6e6a68fe-8f5a-4e49-9428-2446daa94804" />


4. #### 此处代码其内部所包含的就是显示在浏览器上的内容<img width="1177" height="910" alt="屏幕截图 2025-11-11 182030" src="https://github.com/user-attachments/assets/fd6a87a6-08eb-48f7-9691-f2b7f0d91bd3" />


## HTML环境搭建小tips：在VScode中构建HTML环境时可以输入一个！选择只有一个！的那个选项可以直接将结构搭建好

# HTML常用文本标签

- #### 标题标签\<ha>文本\</ha>：a为阿拉伯数字从1到6，字体1最大6最小

- #### 文本标签\<p>文本\</p>：可以在此标签内强调内容,如果想改变段落字体要用到CSS   ~~1~~

- #### 强调标签：\<b>粗体\</b>；\<i>斜体\</i>；\<u>下划线\</u>；\<s>删除线\</s>

- 

- #### 表格标签：最外层用一个\<table>\</table>，\<tr>\</tr>为行，\<td>\<td>为列，\<th>\<th>为表头，还可以将\<table>\</table>改为\<table border="a">\</table>，此操作可以加上边框，a为阿拉伯数字，为边框的宽度

 <img width="304" height="718" alt="屏幕截图 2025-11-11 191817" src="https://github.com/user-attachments/assets/24e7a67f-f599-4f7d-8892-46be68985437" />

<img width="356" height="201" alt="屏幕截图 2025-11-11 191759" src="https://github.com/user-attachments/assets/d5e60d31-ee14-42e3-9b32-8039ee7e980c" />


- #### 列表标签：

  1. #### 无序列表：<img width="339" height="168" alt="屏幕截图 2025-11-11 190619" src="https://github.com/user-attachments/assets/b35bf32e-e0e7-498d-9df9-a07423d695ee" />


  2. #### 有序列表：<img width="334" height="172" alt="屏幕截图 2025-11-11 190627" src="https://github.com/user-attachments/assets/2f052f9f-6877-42bf-819b-e17a38bc38ec" />



- #### 其他标签： 

  1. #### \<br>：相当于回车<img width="715" height="97" alt="屏幕截图 2025-11-11 195338" src="https://github.com/user-attachments/assets/18de0fe0-18ba-49c6-9f48-7e7415f8581c" />

  2. #### \<hr>：创建一个分隔线

# HTML属性

- #### 基本语法<img width="768" height="575" alt="屏幕截图 2025-11-11 192442" src="https://github.com/user-attachments/assets/99a05c63-8350-41ad-bc98-c14cec7caffd" />

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
