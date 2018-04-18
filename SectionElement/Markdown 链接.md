Markdown 链接

Markdown 支持两种形式的链接语法： 行内式和参考式两种形式。不管是哪一种，链接文字都是用 [方括号] 来标记。


行内式链接


要建立一个行内式的链接，只要在方块括号后面紧接着圆括号并插入网址链接即可，如果你还想要加上链接的 title 文字，只要在网址后面，用双引号把 title 文字包起来即可，例如：
<pre>
This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.
</pre>
如果你是要链接到同样主机的资源，你可以使用相对路径
<pre>
See my [About](/about/) page for details.
</pre>
参考式链接


参考式的链接是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记：
<pre>
This is [an example][id] reference-style link.
</pre>
在文件的任意处，你可以把这个标记的链接内容定义出来：
<pre>
[id]: http://example.com/  "Optional Title Here"
</pre>
链接内容定义的形式为：

方括号（前面可以选择性地加上至多三个空格来缩进），里面输入链接文字

   . 接着一个冒号

   . 接着一个以上的空格或制表符

   . 接着链接的网址

   . 选择性地接着 title 内容，可以用单引号、双引号或是括弧包着

下面这三种链接的定义都是相同：
<pre>
[foo]: http://example.com/  "Optional Title Here"
[foo]: http://example.com/  'Optional Title Here'
[foo]: http://example.com/  (Optional Title Here)
</pre>
链接网址也可以用尖括号包起来：
<pre>
[id]: <http://example.com/>  "Optional Title Here"
</pre>
链接辨别标签可以有字母、数字、空白和标点符号，但是并不区分大小写，因此下面两个链接是一样的：
<pre>
[link text][a]
[link text][A]
</pre>
隐式链接标记功能让你可以省略指定链接标记，这种情形下，链接标记会视为等同于链接文字，要用隐式链接标记只要在链接文字后面加上一个空的方括号，如果你要让 "Google" 链接到 google.com，你可以简化成：
<pre>
[Google][]
</pre>
然后定义链接内容：
<pre>
[Google]: http://google.com/
</pre>
下面是一个参考式链接的范例
<pre>
I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"
  </pre>
  如果改成用链接名称的方式写：
  <pre>
I get 10 times more traffic from [Google][] than from
[Yahoo][] or [MSN][].

  [google]: http://google.com/        "Google"
  [yahoo]:  http://search.yahoo.com/  "Yahoo Search"
  [msn]:    http://search.msn.com/    "MSN Search"
  </pre>
  下面是用行内式写的同样一段内容的 Markdown 文件，提供作为比较之用：
  <pre>
  I get 10 times more traffic from [Google](http://google.com/ "Google")
than from [Yahoo](http://search.yahoo.com/ "Yahoo Search") or
[MSN](http://search.msn.com/ "MSN Search").
</pre>
参考式的链接其实重点不在于它比较好写，而是它比较好读，使用 Markdown 的参考式链接，可以让文件更像是浏览器最后产生的结果，让你可以把一些标记相关的元数据移到段落文字之外，你就可以增加链接而不让文章的阅读感觉被打断。


你喜欢哪种链接呢
