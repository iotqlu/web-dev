---
sort: 3
---

# 头部元素

* `<title>`标签
* `<meta>`标签

### `<title>`标签

`<title>`标记在所有 HTML 文档中都是必需的，它定义了文档的标题。

`<title>`元素：

* 在浏览器工具栏中定义标题
* 将页面添加到收藏夹时为其提供标题
* 在搜索引擎结果中显示页面标题

在 index.html 文档中添加`<title>`元素。

index.html 页面的源代码如下：

```html
<!DOCTYPE html>
<html>
  <head>
    <title>HTML Reference</title>
  </head>
</html>
```

### `<meta>`标签

`<meta>`标签数据是有关数据的数据（信息）。

`<meta>`标记始终位于`<head>`元素内，并且它们提供有关 HTML 文档的元数据。

`<meta>`标记通常用于指定字符集，页面描述，关键字，文档的作者和视口设置。

元数据将不会显示在页面上，但是可以在计算机上解析。

浏览器（如何显示内容或重新加载页面），搜索引擎（关键字）和其他 Web 服务都使用元数据。

HTML5 引入了一种方法，使 Web 设计人员可以通过`<meta>`标记来控制视口（用户在网页上的可见区域）（请参见下面的“设置视口”示例）。

| 属性       | 值                                                                                       | 描述                                   |
| ---------- | ---------------------------------------------------------------------------------------- | -------------------------------------- |
| charset    | character_set                                                                            | 指定 HTML 文档的字符编码               |
| content    | text                                                                                     | 给出与 http-equiv 或 name 属性关联的值 |
| http-equiv | content-type <br> default-style <br> refresh                                             | 为内容属性的信息/值提供 HTTP 标头      |
| name       | application-name <br> author <br> description <br> generator <br> keywords <br> viewport | 指定元数据的名称                       |

`<meta>`标签示例：

1. 定义搜索引擎的关键字：

```html
<meta name="keywords" content="HTML, CSS, JavaScript" />
```

2. 定义您的网页描述：

```html
<meta name="description" content="Free Web tutorials for HTML and CSS" />
```

3. 定义页面的作者：

```html
<meta name="author" content="John Doe" />
```

4. 每 30 秒刷新一次文档：

```html
<meta http-equiv="refresh" content="30" />
```

5. 设置视口，以使您的网站在所有设备上看起来都不错：

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

Viewport 是用户在网页上的可见区域。 它随设备的不同而不同-手机上的尺寸要小于计算机屏幕上的尺寸。
以下<meta>元素应该在所有网页中包含：

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

这为浏览器提供了有关如何控制页面尺寸和缩放比例的说明。

`width = device-width`部分将页面的宽度设置为跟随设备的屏幕宽度（视设备而定）。

`initial-scale = 1.0`部分设置浏览器首次加载页面时的初始缩放级别。

实验内容：在`index.html`文件中实验`<meta>`标签。

```checker
- name: check meta tag exist in file index.html
  script: |
    #!/bin/bash
    grep 'meta' /home/project/index.html
  error: 在 index.html 文件中没有找到 &lt;meta&gt; 标签
```
