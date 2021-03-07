---
sort: 8
---

# html5 超链接

本节讲述`<a>`标签。示例：

```html
<a href="https://www.bing.com">Visit Bing!</a>
```

### `<a>`标签

`<a>`标记定义超链接，该超链接用于从一个页面链接到另一页面。

`<a>`元素最重要的属性是`href`属性，它指示链接的目的地。

默认情况下，链接将在所有浏览器中显示如下：

* 未访问的链接带有下划线并显示为蓝色

* 已访问链接带有下划线和紫色

* 活动的链接带有下划线和红色

**注意事项**

* 提示：如果`<a>`标记没有`href`属性，则它只是超链接的占位符。

* 提示：如果`href`属性不存在，则不会显示以下属性：`download`，`hreflang`，`media`，`rel`，`target`和`type`。

* 提示：除非您指定其他目标，否则通常在当前浏览器窗口中显示链接页面。

* 提示：使用`CSS`设置链接样式：`CSS`链接和`CSS`按钮。

**属性**

| 属性           | 值                                                                                                                                                                       | 描述                                                                                                         |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| download       | filename                                                                                                                                                                 | 指定当用户单击超链接时将下载目标。                                                                           |
| href           | URL                                                                                                                                                                      | 指定链接转到的页面的 URL                                                                                     |
| hreflang       | language_code                                                                                                                                                            | 指定链接文档的语言                                                                                           |
| media          | media_query                                                                                                                                                              | 指定链接文档针对哪种媒体/设备进行了优化                                                                      |
| ping           | list_of_URLs                                                                                                                                                             | 指定以空格分隔的 URL 列表，当链接被链接时，带有正文 ping 的发布请求将由浏览器（在后台）发送。 通常用于跟踪。 |
| referrerpolicy | no-referrer <br/> no-referrer-when-downgrade <br/> origin <br/> origin-when-cross-origin <br/> unsafe-url                                                                | 指定要发送的引荐来源                                                                                         |
| rel            | alternate <br/>author <br/> bookmark <br/> external <br/> help <br/> license <br/> next <br/> nofollow <br/> noreferrer <br/> noopener <br/> prev <br/> search <br/> tag | 指定当前文档和链接文档之间的关系                                                                             |
| target         | \_blank <br/>\_parent <br/> \_self <br/>\_top <br/> framename                                                                                                            | 指定在何处打开链接的文档                                                                                     |
| type           | media_type                                                                                                                                                               | 指定链接文档的媒体类型                                                                                       |

