Markdown 特殊字符自动转换

在 HTML 文件中，有两个字符需要特殊处理： < 和 & 。 < 符号用于起始标签，& 符号则用于标记 HTML 实体，如果你只是想要显示这些字符的原型，你必须要使用实体的形式，像是 &lt; 和 &amp;。

& 字符尤其让网络文档编写者受折磨，如果你要打「AT&T」 ，你必须要写成「AT&amp;T」。而网址中的 & 字符也要转换。比如你要链接到：

<pre>
http://images.google.com/images?num=30&q=larry+bird
</pre>
你必须要把网址转换写为：
<pre>
http://images.google.com/images?num=30&amp;q=larry+bird
</pre>
Markdown 让你可以自然地书写字符，需要转换的由它来处理好了。如果你使用的 & 字符是 HTML 字符实体的一部分，它会保留原状，否则它会被转换成 &amp;amp; 。

所以你如果要在文档中插入一个版权符号 ©，你可以这样写：
<pre>
&amp;copy;
</pre>
Markdown 会保留它不动。而若你写：
<pre>
AT&amp;T
</pre>
Markdown 就会将它转为：
<pre>
AT&amp;amp;T
</pre>
类似的状况也会发生在 < 符号上，因为 Markdown 允许 兼容 HTML ，如果你是把 < 符号作为 HTML 标签的定界符使用，那 Markdown 也不会对它做任何转换，但是如果你写：
<pre>
4 < 5
</pre>
Markdown 将会把它转换为：
<pre>
4 &amp;lt; 5
</pre>
不过需要注意的是，code 范围内，不论是行内还是区块， < 和 & 两个符号都一定会被转换成 HTML 实体，这项特性让你可以很容易地用 Markdown 写 HTML code （和 HTML 相对而言， HTML 语法中，你要把所有的 < 和 & 都转换为 HTML 实体，才能在 HTML 文件里面写出 HTML code。）

常用转义字符表为：


|显示结果|描述|实体名称|实体编码|
|:---|:---|:---|:---|
| |空格|&amp;nbsp;|&amp;#160;|
|<|小于号|&amp;lt;|&amp;#60;|
|>|大于号|&amp;gt;|&amp;#62;|
|&|和号|&amp;amp;|&amp;#38;|
|“|引号|&amp;quot;|&amp;#34;|
|‘|撇号|&amp;apos;(IE不支持)|&amp;#39;|

