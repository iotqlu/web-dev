---
sort: 7
---


# html5 多媒体

使用 html5 多媒体标签可以在文档中添加图像、音频、视频内容。

### html5图像标签`<img>`

`<img>`标签

```html
<img
  src="https://pic1.zhimg.com/v2-e327160ba23d1bc7c457b63798b85a69_1200x500.jpg"
  alt="Smiley face"
  height="420"
/>
```

`<img>`标记在 HTML 页面中定义图像。

`<img>`标记具有两个必需的属性：`src`和`alt`。

注意：从技术上讲，图像不是插入到 HTML 页面中，而是将图像链接到 HTML 页面。 `<img>`标签为引用的图像创建一个容纳空间。

提示：要将图像链接到另一个文档，只需将`<img>`标记嵌套在`<a>`标记内。

### html5 音视频

`<audio>`标签定义声音，例如音乐或其他音频流。

当前，`<audio>`元素支持 3 种文件格式：`MP3`，`WAV`和`OGG`：

`<audio>`示例：

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg" />
  <source src="horse.mp3" type="audio/mpeg" />
  Your browser does not support the audio tag.
</audio>
```

提示：`<audio>`和`</audio>`之间的任何文本将在不支持`<audio>`标记的浏览器中显示。

`<video>`标签指定视频，例如影片剪辑或其他视频流。

当前，`<video>`元素支持 3 种视频格式：`MP4`，`WebM`和`Ogg`：

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4" />
  <source src="movie.ogg" type="video/ogg" />
  Your browser does not support the video tag.
</video>
```

提示：`<video>`和`</video>`标记之间的所有文本将在不支持`<video>`
元素的浏览器中显示.