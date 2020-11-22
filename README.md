# Electron

### [Electron官方文档 https://www.electronjs.org](https://www.electronjs.org/)

>  使用 JavaScript，HTML 和 CSS 构建跨平台的桌面应用程序
>
> ### 比你想象的更简单
>
> 如果你可以建一个网站，你就可以建一个桌面应用程序。 Electron 是一个使用 JavaScript, HTML 和 CSS 等 Web 技术创建原生程序的框架，它负责比较难搞的部分，你只需把精力放在你的应用的核心上即可。



基本的Electron应用程序仅需要以下文件：

- `package.json` - 指向应用程序的主文件，并列出其详细信息和依赖项。
- `main.js` - 启动应用程序并创建一个浏览器窗口以呈现HTML。 这是应用程序的“主要进程”。
- `index.html` - 要呈现的网页。 这是应用程序的“渲染程序”



### 控制台乱码怎么解决：

数字表示的字符集。而常见的gb2312的值是936，utf8的值是65001

``` js
# 在package.json中的scripts中添加 chcp 65001 === utf8

"scripts": {
    "start": "chcp 65001 && electron ."
 },
```



