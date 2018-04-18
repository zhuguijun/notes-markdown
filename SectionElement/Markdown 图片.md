Markdown 图片

很明显地，要在纯文字应用中设计一个「自然」的语法来插入图片是有一定难度的。

Markdown 使用一种和链接很相似的语法来标记图片，同样也允许两种样式： 行内式和参考式。

行内式的图片语法看起来像是:
<pre>
![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")
</pre>
有没有似曾相识，和链接的语法是不是很像


图片语法如下：


&emsp;. 一个惊叹号 !

&emsp;. 接着一个方括号，里面放上图片的替代文字

&emsp;. 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上 选择性的 'title' 文字。

参考式的图片语法则长得像这样：
<pre>
![Alt text][id]
</pre>
「id」是图片参考的名称，图片参考的定义方式则和链接参考一样，回顾下链接参考语法：
<pre>
[id]: url/to/image  "Optional title attribute"
</pre>

