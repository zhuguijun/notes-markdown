Markdown 表格

语法说明：

1. 不管是哪种方式，第一行为表头，第二行分隔表头和主体部分，第三行开始每一行为一个表格行。
2. 列于列之间用管道符|隔开。原生方式的表格每一行的两边也要有管道符。
3. 第二行还可以为不同的列指定对齐方向。默认为左对齐，在-右边加上:就右对齐。

代码：

简单方式写表格：
<pre>
学号|姓名|分数
-|-|-
小明|男|75
小红|女|79
小陆|男|92
</pre>
原生方式写表格：
<pre>
|学号|姓名|分数|
|-|-|-|
|小明|男|75|
|小红|女|79|
|小陆|男|92|
</pre>

显示效果： 

|学号|姓名|分数|
|-|-|-|
|小明|男|75|
|小红|女|79|
|小陆|男|92|

表格对齐格式
<pre>
居左：:----
居中：:----:或-----
居右：----:
</pre>

例子：
<pre>
|标题|标题|标题|
|:---|:---:|---:|
|居左测试文本|居中测试文本|居右测试文本|
|居左测试文本1|居中测试文本2|居右测试文本3|
|居左测试文本11|居中测试文本22|居右测试文本33|
|居左测试文本111|居中测试文本222|居右测试文本333|
</pre>

效果如下：


|标题|标题|标题|
|:---|:---:|---:|
|居左测试文本|居中测试文本|居右测试文本|
|居左测试文本1|居中测试文本2|居右测试文本3|
|居左测试文本11|居中测试文本22|居右测试文本33|
|居左测试文本111|居中测试文本222|居右测试文本333|
