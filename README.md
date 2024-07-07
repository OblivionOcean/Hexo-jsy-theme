# Hexo-jsy-theme

#### 介绍

一个简洁的hexo主题

#### 软件架构

采用ejs模板生成器，模板使用jquery、bootstrap


#### 版权声明

采用GPL3.0许可证，请您遵守许可证规则并在项目中注明本仓库地址

备注：本项目已转移至玄云海团队（oboc）

#### 安装教程

1.  clone本仓库到本地
2.  写文章、改友链
3.  推送到服务器或github page

#### 使用说明

0. 配置好hexo环境，记得装个wordcount插件，自行百度，过程比较简单就不多说了

1.  Clone步骤：本仓库是一个JSY主题的博客示例，你可以选择仅使用theme文件夹内的主题，也可以选择使用整个仓库并修改
2.  首先修改`/_config.yml`中的内容，设置`theme: jsy`，设置`title: 博客名称`，设置`subtitle: 副标题`，设置`description：博客介绍`，设置`author: 你的名字`
3. 接着找到`/_config.jsy.yml`（注意是根目录下的那个），设置`about: 你的个人介绍`和`avatar: 你的头像链接`
4. 然后找到`/source/links/index.md`，按照下述格式添加友链：

```yml
---
title: 友情链接
---

<a href="https://友链1的网址">
<div class="friend">
<h2>友链1 的名称</h2>
<h3>友链1 的介绍</h3>
</div>
</a>

<a href="https://友链2的网址">
<div class="friend">
<h2>友链2 的名称</h2>
<h3>友链2 的介绍</h3>
</div>
</a>
```

你可以按照自身需求添加和更改

5. 好了，现在找到`/source/_posts`目录，在目录下新建一个markdown文件（如：hello.md），按照下述格式写文章：

```yml
---
title: 文章标题
---
这里写上你的文章内容
可以使用markdown语法
```

写好之后保存

6. 最后，在命令行执行以下命令：

（
如果你是第一次使用，请先运行以下命令
```sh
hexo new page 404
```
）

```sh
hexo cl
hexo g
```

执行后等待生成，在public目录下可以找到生成的静态文件，把它放到服务器或者github page上就搞定了！

（如果404页面显示的是默认页面，您可以修改服务器配置将404页面指向`/404`）