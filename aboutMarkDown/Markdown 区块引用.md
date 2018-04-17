Markdown 标记区块引用是使用类似 email 中用 > 的引用方式。如果你还熟悉在 email 信件中的引言部分，你就知道怎么在 Markdown 文件中建立一个区块引用，那会看起来像是你自己先断好行，然后在每行的最前面加上 > ：
<pre>
> something about markdown,
> something about markdown.
> something about markdown.
> 
> something about markdown
> something about markdown.
</pre>

Markdown 也允许你偷懒只在整个段落的第一行最前面加上 > ：
<pre>
> 和程序相关的写作或是标签语言原始码通常会有已经排版好的代码区块，
通常这些区块我们并不希望它以一般段落文件的方式去排版，
而是照原来的样子显示，Markdown 会用 &ltpre> 和 &ltcode> 标签来把代码区块包起来。

> 要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以。
</pre>

区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 > ：


<pre>
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
<pre>

引用的区块内也可以使用其他的 Markdown 语法，包括标题、列表、代码区块等：
<pre>
> ## 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");
</pre>
