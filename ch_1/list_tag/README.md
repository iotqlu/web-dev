---
sort: 7
---


# html5 列表

| 标签   | 描述             |
| ------ | ---------------- |
| `<ol>` | 有序列表         |
| `<ul>` | 无序列表         |
| `<li>` | 列表项           |
| `<dl>` | 定义列表         |
| `<dt>` | 定义列表项目     |
| `<dd>` | 定义列表项目描述 |

### 有序列表

`<ol>`标记定义一个有序列表。 有序列表可以是数字或字母。

使用`<li>`标记定义列表项。

两个不同的有序列表（第一个列表从 1 开始，第二个列表从 50 开始）：

```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

### 无序列表

`<ul>`标记定义了无序列表（项目符号）。

将`<ul>`标记与`<li>`标记一起使用可创建无序列表。

示例：

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

### 定义列表

`<dl>`标记定义描述列表。

`<dl>`标记与`<dt>`（定义术语/名称）和`<dd>`（描述每个术语/名称）一起使用。

示例：描述列表，其中包含术语和描述：

```html
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```