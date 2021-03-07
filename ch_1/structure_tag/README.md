---
sort: 5
---

# 文档结构标签

html5 结构标签用于搭建页面主体内容结构，形成不同的区块，完成整个页面的排版布局。

| 标签        | 描述                            |
| ----------- | ------------------------------- |
| `<article>` | 定义文章                        |
| `<aside>`   | 定义页面内容之外的内容          |
| `<details>` | 定义元素的细节                  |
| `<footer>`  | 定义 section 或 page 的页脚     |
| `<header>`  | 定义 section 或 page 的页眉     |
| `<nav>`     | 定义导航链接                    |
| `<section>` | 定义 section                    |
| `<summary>` | 为`<details>`元素定义可见的标题 |
| `<div>`     | 定义文档中的节                  |
| `<span>`    | 定义文档中的行内元素            |

```html
<article>
  <header>
    <h1>Most important heading here</h1>
    <h2>Less important heading here</h2>
    <p>Some additional information here</p>
  </header>
  <p>Lorem Ipsum dolor set amet....</p>
</article>
```

实验内容：在```index.html```文件中实验```<header>```标签。


```checker
- name: check header tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'header' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;header&gt; 标签
```

### `<header>`标签

`<header>`元素表示介绍性内容或一组导航链接的容器。

`<header>`元素通常包含：

* 一个或多个标题元素（`<h1>`-`<h6>`）
* 徽标或图标
* 作者信息

一个文档中可以包含多个`<header>`元素。

注意：`<header>`标记不能放在`<footer>`，`<address>`或另一个`<header>`元素内。

示例：

```html
<article>
  <header>
    <h1>Most important heading here</h1>
    <h2>Less important heading here</h2>
    <p>Some additional information here</p>
  </header>
  <p>Lorem Ipsum dolor set amet....</p>
</article>
```



### `<nav>`标签

`<nav>`标记定义了一组导航链接。

请注意，并非文档的所有链接都应在`<nav>`元素内。 `<nav>`元素仅用于主要的导航链接块。

浏览器（例如，供残障用户使用的屏幕阅读器）可以使用此元素来确定是否忽略此内容的初始呈现。

示例：

```html
<nav>
  <a href="/html/">HTML</a> | <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav>
```

```checker
- name: check nav tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'nav' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;nav&gt; 标签
```

### `<article>`标签

`<article>`标记指定独立的，独立的内容。

文章应该是有意义的，并且有可能独立于网站的其余部分进行分发。

`<article>`元素的潜在来源：

* 论坛帖子
* 博客文章
* 新闻故事
* 评论

示例：

```html
<article>
  <h2>Google Chrome</h2>
  <p>
    Google Chrome is a web browser developed by Google, released in 2008. Chrome
    is the world's most popular web browser today!
  </p>
</article>

<article>
  <h2>Microsoft Edge</h2>
  <p>
    Microsoft Edge is a web browser developed by Microsoft, released in 2015.
    Microsoft Edge replaced Internet Explorer.
  </p>
</article>
```

```checker
- name: check article tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'article' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;article&gt; 标签
```

### `<section>`标签

`<section>`标记定义文档中的各个部分，例如章节，页眉，页脚或文档的任何其他部分。

示例：

文档中的一节，说明什么是 WWF：

```html
<section>
  <h2>WWF</h2>
  <p>The World Wide Fund for Nature (WWF) is....</p>
</section>
```

```checker
- name: check section tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'section' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;section&gt; 标签
```

### `<aside>`标签

`<aside>`标记定义了放置内容以外的内容。

预留内容应与周围的内容有关。

示例：

```html
<p>
  My family and I visited The Epcot center this summer. The weather was nice,
  and Epcot was amazing! I had a great summer together with my family!
</p>

<aside>
  <h4>Epcot Center</h4>
  <p>
    Epcot is a theme park at Walt Disney World Resort featuring exciting
    attractions, international pavilions, award-winning fireworks and seasonal
    special events.
  </p>
</aside>
```

```checker
- name: check aside tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'aside' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;aside&gt; 标签
```

### `<footer>`标签

`<footer>`标记定义文档或节的页脚。

`<footer>`元素通常包含：

* 作者信息
* 版权信息
* 联系信息
* 网站地图
* 回到顶部链接
* 相关文件

一个文档中可以包含多个`<footer>`元素。

示例：

```html
<footer>
  <p>Posted by: Hege Refsnes</p>
  <p>
    Contact information:
    <a href="mailto:someone@example.com"> someone@example.com</a>.
  </p>
</footer>
```

```checker
- name: check footer tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'footer' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;footer&gt; 标签
```

### `<details>`和`<summary>`标签

`<details>`标签指定用户可以按需查看或隐藏的其他详细信息。

`<details>`标签可用于创建用户可以打开和关闭的交互式窗口小部件。 任何种类的内容都可以放在`<details>`标记内。

除非设置了 open 属性，否则`<details>`元素的内容应该不可见。

`<summary>`标记为`<details>`元素定义了可见的标题。 可以单击标题以查看/隐藏详细信息。

指定用户可以按需查看或隐藏的详细信息：

```html
<details>
  <summary>Copyright 1999-2018.</summary>
  <p>- by Refsnes Data. All Rights Reserved.</p>
  <p>
    All content and graphics on this web site are the property of the company
    Refsnes Data.
  </p>
</details>
```

```checker
- name: check details tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'details' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;details&gt; 标签
```

```checker
- name: check summary tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'summary' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;summary&gt; 标签
```

### `<div>`标签

文档中具有浅蓝色背景色的部分：

```html
<div style="background-color:lightblue">
  <h3>This is a heading</h3>
  <p>This is a paragraph.</p>
</div>
```

`<div>`标记定义 HTML 文档中的分区或部分。

`<div>`元素通常用作其他 HTML 元素的容器，以使用 CSS 对其进行样式设置或使用 JavaScript 执行某些任务。

```checker
- name: check div tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'div' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;div&gt; 标签
```

### `<span>`标签

使用`<span>`标签定义文本颜色

```html
<p>My mother has <span style="color:blue">blue</span> eyes.</p>
```

`<span>`标记是一个内联容器，用于标记文本的一部分或文档的一部分。

`<span>`标记本身并没有提供视觉上的变化，但是标记后，您可以使用 CSS 设置样式或使用 JavaScript 对其进行操作。

```checker
- name: check span tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'span' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;span&gt; 标签
```