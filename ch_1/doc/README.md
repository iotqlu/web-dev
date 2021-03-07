---
sort: 2
---

# 文档结构元素

新建文件`index.html`，添加 html5 文档类型声明，源代码如下：

```html
<!DOCTYPE html>
<html></html>
```

在 html5 文档中，文档类型声明`<!DOCTYPE>`是强制使用的，必须位于文档首行，浏览器才能获知文档类型。`<!DOCTYPE>`声明不是 html 标签，浏览器通过`<!DOCTYPE>`声明判断 html 文档使用的 html 版本，`<!DOCTYPE html>`声明使用的是 html5 的版本。

之前 html 版本的声明如下:

`HTML 4.01:`

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

`XHTML 1.1:`

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
```

* `<html>`标签
* `<head>`标签
* `<body>`标签

`<html>`与`</html>`标签定义了文档的开始和结束，文档由头部和主体组成，文档的头部由`<head>`标签定义，主体由`<body>`标签定义。

在`index.html`文件中添加`<head>`和`<body>`标签。

index.html 页面的源代码如下：

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    Hello World!
  </body>
</html>
```
如下图所示，预览index.html文档内容，后续实验内容，请自行实验每一个html5标签，并在预览界面中查看显示效果。
![新建index.html文档](../assets/ch_1/1.jpg)

```checker
- name: check index.html exist
  script: |
    #!/bin/bash
    ls -l /home/project/index.html
  error: 没有找到 /home/project/index.html 文件
```