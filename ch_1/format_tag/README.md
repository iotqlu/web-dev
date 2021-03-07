---
sort: 6
---

# html5 格式化标签

* 文本格式化标签
* 引用和术语定义标签
* html5 新增格式化标签

### 文本格式化标签

| 标签    | 描述                         |
| ------- | ---------------------------- |
| `<sub>` | 下标文本                     |
| `<sup>` | 上标文本                     |
| `<ins>` | 插入文本                     |
| `<del>` | 删除文本                     |
| `<wbr>` | 定义在文本何处适合添加换行符 |
| `<pre>` | 预设格式文本                 |

示例：

```html
<p>This text contains <sub>subscript</sub> text.</p>

<p>This text contains <sup>superscript</sup> text.</p>

<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>

<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>

<p>
  To learn AJAX, you must be familiar with the XML<wbr />Http<wbr />Request
  Object.
</p>

<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>
```

### 引用和术语定义标签

| 标签           | 描述       |
| -------------- | ---------- |
| `<abbr>`       | 缩写       |
| `<address>`    | 地址       |
| `<bdo>`        | 文字方向   |
| `<blockquote>` | 长的引用语 |
| `<q>`          | 短的引用语 |

示例：

```html
The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.

<address>
  Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br />
  Visit us at:<br />
  Example.com<br />
  Box 564, Disneyland<br />
  USA
</address>

<bdo dir="rtl">
  This text will go right-to-left.
</bdo>

<blockquote cite="http://www.worldwildlife.org/who/index.html">
  For 50 years, WWF has been protecting the future of nature. The world's
  leading conservation organization, WWF works in 100 countries and is supported
  by 1.2 million members in the United States and close to 5 million globally.
</blockquote>

<p>
  WWF's goal is to:
  <q>Build a future where people live in harmony with nature.</q>
  We hope they succeed.
</p>
```