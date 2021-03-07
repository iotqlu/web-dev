---
sort: 4
---

# html5 基础标签

| 标签        | 描述            |
| ----------- | --------------- |
| `<h1>~<h6>` | 标题 1 至标题 6 |
| `<p>`       | 定义段落        |
| `<br>`      | 换行            |
| `<hr>`      | 水平线          |
| `<!-->`     | 注释            |

### `<h1>~<h6>`

`<h1>`到`<h6>`标记用于定义 HTML 标题。

`<h1>`定义最重要的标题。 `<h6>`定义最不重要的标题。

```html
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6>
```

### `<p>`

`<p>`标记定义一个段落。

浏览器会在每个`<p>`元素之前和之后自动添加一些空间（边距）。 可以使用 CSS（带有 margin 属性）修改页边距。

```html
<p>This is some text in a paragraph.</p>
```

### `<br>`

`<br>`标签插入了一个换行符。

`<br>`标签是一个空标签，这意味着它没有结束标签。

```html
<p>
  To force<br />
  line breaks<br />
  in a text,<br />
  use the br<br />
  element.
</p>
```

### `<hr>`

`<hr>`标记定义 HTML 页面中的主题中断（例如，主题转移）。

`<hr>`元素通常显示为水平规则，用于分隔 HTML 页面中的内容（或定义更改）。

```html
<h1>HTML</h1>
<p>HTML is a language for describing web pages.....</p>

<hr />

<h1>CSS</h1>
<p>CSS defines how to display HTML elements.....</p>
```

### 注释标签

comment 标签用于在源代码中插入注释。 注释不会显示在浏览器中。

您可以使用注释来解释代码，以便日后编辑源代码时为您提供帮助。 如果您有很多代码，这特别有用。

```html
<!--This is a comment. Comments are not displayed in the browser-->

<p>This is a paragraph.</p>
```