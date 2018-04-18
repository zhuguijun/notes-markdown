Markdown 强调

Markdown 使用星号（*）和底线（_）作为标记强调字词的符号，被 * 或 _ 包围的字词会被转成用 &lt;em> 标签包围，用两个 * 或_ 包起来的话，则会被转成 &lt;strong>，例如：
<pre>
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__
</pre>
会转成：
<pre>
&lt;em>single asterisks&lt;/em>

&lt;em>single underscores&lt;/em>

&lt;strong>double asterisks&lt;/strong>

&lt;strong>double underscores&lt;/strong>
</pre>
你可以随便用你喜欢的样式，唯一的限制是，你用什么符号开启标签，就要用什么符号结束。

强调也可以直接插在文字中间：

<pre>
un*frigging*believable
</pre>
但是如果你的 * 和 _ 两边都有空白的话，它们就只会被当成普通的符号。如果要在文字前后直接插入普通的星号或底线，你可以用反斜线：
<pre>
\*this text is surrounded by literal asterisks\*
</pre>

这样的简便你喜欢吗
