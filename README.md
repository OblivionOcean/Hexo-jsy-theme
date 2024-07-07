# Hexo-jsy-theme

![Cover](https://github.com/Lafcadia/Hexo-jsy-theme/assets/147896059/312c0bcb-6a3e-4aa6-b933-f8f5a424464b)


#### 介绍

一个简洁，易用的 Hexo 主题。

#### 架构

采用 EJS 模板生成器，模板使用 JQuery, Bootstrap。

#### 版权声明

采用 GPL 3.0 许可证，使用时请您遵守许可证规则，并在项目中注明本仓库地址。

#### 安装 & 使用

1. 克隆到博客根目录下的 `themes` 文件夹。示例：
   ```shell
   git clone https://github.com/OblivionOcean/Hexo-jsy-theme.git /themes/jsy
   ```
2. 修改友链等使其符合本主题格式。
3. 推送到服务器或 Github Page (见 [Hexo 官方教程](https://hexo.io/docs/one-command-deployment))

#### 使用说明

0. 配置好 Hexo 环境 (见[Hexo 官方教程](https://hexo.io/docs/setup)，记得装个 wordcount 插件 (在博客根目录执行 `cnpm i --save hexo-wordcount`)

1. Clone 步骤：本仓库是一个JSY主题的博客示例，你可以选择仅使用theme文件夹内的主题，也可以选择使用整个仓库并修改
2. 首先修改 `/_config.yaml` 中的内容: 
   ```yaml
   title: 博客名称
   subtitle: 副标题
   description：博客介绍
   author: 你的名字
   theme: jsy
   ```
3. 接着找到 `/_config.jsy.yaml`（博客根目录下）:
   ```yaml
   about: 你的个人介绍
   avatar: 你的头像链接
   ```
4. 然后找到 `/source/links/index.md`，按照下述格式添加友链：

  ```markdown
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

你可以按照自身需求添加和更改友链。

5. 打开 `/source/_posts` 目录，在目录下新建一个 Markdown 文件（如：`hello.md`），按照下述格式书写文章：

```markdown
---
title: 文章标题
---
<!--此段为正文，请使用 Markdown 语法。-->
```

写好之后保存。

6. 在命令行执行以下命令：

(如果你是第一次使用，请先运行以下命令: `hexo new page 404`)

`hexo clean && hexo g -d`

执行后等待静态文件生成，在 `public` 目录下可以找到生成的静态文件，把它部署到服务器或者 Github Page。

（P.S. 如果 404 页面显示的是默认页面，您可以修改服务器配置将 404 页面指向 `/404`。）
