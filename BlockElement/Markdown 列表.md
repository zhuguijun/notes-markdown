Markdown 支持有序列表和无序列表。

无序列表使用星号、加号或是减号作为列表标记
<pre>
*   Red
*   Green
*   Blue
</pre>


等同于：
<pre>
+   Red
+   Green
+   Blue
</pre>


也等同于：
<pre>
-   Red
-   Green
-   Blue
</pre>

有序列表则使用数字接着一个英文句点：
<pre>
1.  Bird
2.  McHale
3.  Parish
</pre>
很重要的一点是，你在列表标记上使用的数字并不会影响输出的 HTML 结果，上面的列表所产生的 HTML 标记为：
<pre>
<ol>
<li>Bird</li>
<li>McHale</li>
<li>Parish</li>
</ol>
</pre>
如果你的列表标记写成：
<pre>
1.  Bird
1.  McHale
1.  Parish
</pre>
或甚至是：
<pre>
3. Bird
1. McHale
8. Parish
</pre>

如果列表项目间用空行分开，在输出 HTML 时 Markdown 就会将项目内容用 &lt;<p> 标签包起来，举例来说：
<pre>
 *   Bird

*   Magic
</pre>

会被转换为：
<pre>
<ul>
<li><p>Bird</p></li>
<li><p>Magic</p></li>
</ul>
</pre>

列表项目可以包含多个段落，每个项目下的段落都必须缩进 4 个空格或是 1 个制表符：
<pre>
1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.
</pre>

如果要在列表项目内放进引用，那 > 就需要缩进：
<pre>
*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.
</pre>

如果要放代码区块的话，该区块就需要缩进两次，也就是 8 个空格或是 2 个制表符：
<pre>
*   一列表项包含一个列表区块：

        <代码写在这>
</pre>
