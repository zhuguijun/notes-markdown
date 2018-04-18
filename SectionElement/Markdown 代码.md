Markdown 代码

如果要标记一小段行内代码，你可以用反引号把它包起来（`），例如：
<pre>
Use the `printf()` function.
</pre>
如果要在代码区段内插入反引号，你可以用多个反引号来开启和结束代码区段：
<pre>
``There is a literal backtick (`) here.``
</pre>
这段语法会产生：
<pre>
<p><code>There is a literal backtick (`) here.</code></p>
</pre>
在代码区段内，& 和尖括号都会被自动地转成 HTML 实体，这使得插入 HTML 原始码变得很容易，Markdown 会把下面这段：
<pre>
Please don't use any `<blink>` tags.
</pre>
转为:
<pre>
&lt;p>Please don't use any &lt;code>&lt;blink&gt;&lt;/code> tags.&lt;/p>
</pre>
