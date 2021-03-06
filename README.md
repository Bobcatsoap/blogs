拼文博客系统
----------

## Fork 本库，建立自己的博客系统

操作步骤如下：

第 1 步，在 github.com 打开本库，即 [rewgt/blogs](https://github.com/rewgt/blogs)，点击右上角的 fork 按钮，将本库 fork 到您自己的账号下。

第 2 步，在本机安装 shadow-widget 运行环境

``` bash
mkdir user
cd user
git clone https://github.com/rewgt/shadow-server.git
```

第 3 步，在本机克隆刚 fork 过来的 blogs 项目

``` bash
git clone https://github.com/<your_account>/blogs.git
```

第 4 步，在本机创建博客

在本机启动一个 server：

``` bash
cd shadow-server
npm install
npm start
```

然后在浏览器访问 blogs 主页：`http://localhost:3000/blogs/`，创建、编辑、管理博客在该主页下进行。发布博客只需用 `git push` 命令把本机的 repository 提交到 github 的 `gh-pages` 分支。

当您有博客 push 到 github 后，应能按如下地址访问自己的 github 博客主页：

```
https://<your_account>.github.io/blogs/
```

请自行替换上面 URL 中的 `"<your_account>"`，当然，您还应修改 `README.md` 文件，删除无关内容，并公布自己博客主页的链接。

## 使用限制

本博客系统的客户端支持用主流浏览器访问，包括 Safari、Chrome、Firefox、IE、Opera 等，其中 IE 要求用 IE9 以上版本。对浏览器的最低要求正是 React 所提的要求，也与您撰写的文章是否用到特定 Web 特性有关，如果只用 markdown 编写简单的文档，遵循 React 最低运行环境的规定即可。如果您撰写文章深度依赖 HTML5 特性，比如绘制 chart 统计图，在客户端阅读时，IE 浏览器最好用 IE11 以后的版本（包括 Edge），其它浏览器也最好是近两年发布的版本。

本博客系统不只用浏览器阅读文章，也用它编辑文章。浏览器用作编辑时，IE 限用 Edge 以上的版本，因为太多 "IE Rocks"，只有 `Edge+` 才支持 Shadow Widget 的可视化设计器。其它主流浏览器则没什么特别要求，版本不要过于老旧即可。另外，编辑文章在本机进行，因启动一个 localhost 的 Web 服务，这要求在本机预装 NodeJs 与 NPM 运行环境。

## 帮助文档

本库博客地址：<a target="_blank" rel="noopener" href="https://rewgt.github.io/blogs/">https://rewgt.github.io/blogs/</a>，如何撰写拼文，如何管理博客，如何提交等，在此博客的 `"Online help"` 子项里有介绍。

<a target="_blank" rel="noopener" href="https://rewgt.github.io/blogs/output/doc/doc_zh/">点击这里阅读 PINP Blog 开发者手册</a>

## 版权

本库采用 WTFPL 协议（Do What The Fuck You Want To Public License）。

本库的本地编辑环境依赖于 [`shadow-server`](https://github.com/rewgt/shadow-server) 项目，`shadow-server` 按 `BSD 3-clause` 协议开源。

&nbsp;
