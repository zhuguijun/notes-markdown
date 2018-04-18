Markdown 兼容 HTML

Markdown 不是想要取代 HTML，甚至也没有要和它相近，它的语法种类很少，只对应 HTML 标记的一小部分。Markdown 的构想不是要使得 HTML 文档更容易书写。在我看来， HTML 已经很容易写了。Markdown 的理念是，能让文档更容易读、写和随意改。HTML 是一种发布的格式，Markdown 是一种书写的格式。就这样，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。不需要额外标注这是 HTML 或是 Markdown；只要直接加标签就可以了。

要制约的只有一些 HTML 区块元素――比如 &lt;div>、&lt;table>、&lt;pre>、&lt;p> 等标签，必须在前后加上空行与其它内容区隔开，还要求它们的开始标签与结尾标签不能用制表符或空格来缩进。Markdown 的生成器有足够智能，不会在 HTML 区块标签外加上不必要的 <p> 标签。

例子如下，在 Markdown 文件里加上一段 HTML 表格：
<pre>
这是一个普通段落。

&lt;table>
    &lt;tr>
        &lt;td>Foo&lt;/td>
    &lt;/tr>
&lt;/table>

这是另一个普通段落。
</pre>
请注意，在 HTML 区块标签间的 Markdown 格式语法将不会被处理。比如，你在 HTML 区块内使用 Markdown 样式的\*强调\*会没有效果。

HTML 的区段（行内）标签如 &lt;span>、&lt;cite>、&lt;del> 可以在 Markdown 的段落、列表或是标题里随意使用。依照个人习惯，甚至可以不用 Markdown 格式，而直接采用 HTML 标签来格式化。举例说明：如果比较喜欢 HTML 的 &lt;a> 或 &lt;img> 标签，可以直接使用这些标签，而不用 Markdown 提供的链接或是图像标签语法。

和处在 HTML 区块标签间不同，Markdown 语法在 HTML 区段标签间是有效的

对会编写html格式的小伙伴来说，是不是搜 so&nbsp;easy： 


<div style={{background-color:red}}>
    
<mark>this is div start</mark>
  
this.is div content

<mark>this is div end</mark>
 
</div>

<h3><del>this is h3 but is replace</del></h3>   
<h4>this is h4</h4>
<p>指数幂示例:</p>
<p>2<sup>0</sup>=1;</p>
<p>2<sup>1</sup>=2;</p>
<p>2<sup>2</sup>=4;</p>
