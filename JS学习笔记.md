# JS的导入方式

1. #### 可以在head，body中用\<script>\</script>写入JS

2. #### 外联样式：于CSS的外联样式步骤相同但引入时用

   #### \<script src="文件路径">\</script>

   

# 函数

#### 依旧是在\<script>\</script>中写入函数值，与c语言的函数用法是相同的

#### function functionname(参数值){

​     

#### }

#### 此处参数不相同于除了语言那么严谨，不用定义参数的类型，直接写参数名即可，如

#### function hello(name){

#### console.log('hello', + name);

#### }

#### hello(world);

#### 会输出hello，world

#### 此处的console.log()浏览器控制台中相当于c语言printf，此处还可以使用alert()直接以警告的形式显示在网页上

# JS语法

#### 几乎与c语言相通

# 事件

#### 指文档或浏览器窗口中发生的特定瞬间，例如用户的点击，键盘的按下，页面的加载等

# 事件绑定

#### 函数出发的条件就是事件，当事件被触发就会调用相应的函数![image-20251116165840172](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251116165840172.png)

#### 第一列都是属性，他们的属性值是相应行为绑定的函数名

# DOM 