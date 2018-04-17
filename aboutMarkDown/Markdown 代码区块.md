和程序相关的写作或是标签语言原始码通常会有已经排版好的代码区块，通常这些区块我们并不希望它以一般段落文件的方式去排版，而是照原来的样子显示，Markdown 会用 &lt;pre> 和 &lt;code> 标签来把代码区块包起来。

要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以，例如，下面的输入：
<pre>
这是一个普通段落：

    这是一个代码区块。
</pre>

这个每行一阶的缩进（4 个空格或是 1 个制表符），都会被移除，例如：
<pre>
Here is an example of script:

    tell application "Foo"
        beep
    end tell
</pre>

会被转换为：
<pre>
&lt;p>Here is an example of script:&lt;/p>

&lt;pre>&lt;code>tell application "Foo"
    beep
end tell
&lt;/code>&lt;/pre>
</pre>
一个代码区块会一直持续到没有缩进的那一行（或是文件结尾）。


在代码区块里面， &amp;、 &lt; 和 > 会自动转成 HTML 实体，这样的方式让你非常容易使用 Markdown 插入范例用的 HTML 原始码，只需要复制贴上，再加上缩进就可以了，剩下的 Markdown 都会帮你处理，例如：
<pre>
    &lt;div class="footer">
        &amp;copy; 2004 Foo Corporation
    &lt;/div>
</pre>
会被转换为：
<pre>
&lt;pre>&lt;code>&lt;div class="footer"&gt;
    &amp;copy; 2004 Foo Corporation
&lt;/div&gt;
&lt;/code>&lt;/pre>
</pre>
代码区块中，一般的 Markdown 语法不会被转换，像是星号便只是星号，这表示你可以很容易地以 Markdown 语法撰写 Markdown 语法相关的文件。
