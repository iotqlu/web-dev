---
sort: 0
---

# 开发环境

Web开发基础实验课程主要针对静态网站开发技术的学习和实践, 开发环境可以采用桌面IDE和Web服务器相结合的方式实现.

可以采用的IDE, 如: Eclipse, VS Code, Notepad++等

可以采用的Web服务器, 如: Tomcat, Apache, Ngnix, IIS, Python等.

Web应用运行于桌面浏览器, 如: Firefox, Chrome, IE, Safari等.

**推荐的开发环境:**

* IDE使用VS Code
* 浏览器使用Firefox或Chrome
* Web服务器使用VS Code自带的Live Server

## 快速入门

1. 选择一个开发使用的文件夹, 在这个文件夹下新建一个文件夹作为工程目录, 如: webdev.
1. 打开VS Code, 使用`File -> Add Folder to Workspace`功能将webdev文件夹添加到VS Code中.
1. 新建一个文件, 命令为: `index.html`, 文件中编写以下代码: 

    ```html
    <!DOCTYPE HTML>
    <body>
    Hello World
    </body>
    ```

1. 右键单击`index.html`文件, 选择 `Open with Live Server`, 会自动打开系统默认的浏览器并访问地址: `http://127.0.0.1:5500/index.html`. 注: 这里的端口号可能会不同, VS Code会提示使用的端口号.
1. 修改`index.html`文件的内容, 保存文件后, 浏览器中的页面效果会自动刷新.