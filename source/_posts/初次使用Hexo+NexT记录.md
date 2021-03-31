---
title: 初次使用Hexo+NexT记录
categories: 使用记录
tags:
   - Hexo
   - NexT
   - 使用记录
---
> 一直都知道github pages可以搭建个人博客，这是第一次上手搭建并使用，就把搭建本博客的过程做一次记录吧！


## `Hexo`的安装

1. Hexo环境搭建需要安装Git+NodeJs，根据官网操作安装即可。
    - [Git官网](https://git-scm.com/)
    - [NodeJs官网](https://nodejs.org/zh-cn/)

2. 开始安装`Hexo`

    - [Hexo官网](https://hexo.io/zh-cn/)

   ```bash
   # 全局安装hexo
   npm install hexo-cli -g
   ```

3. 安装主题Next

    - [Next官网](https://theme-next.iissnan.com/)

## `Hexo`的使用

新建一个工程

```bash
hexo init <folder>
```

安装依赖

```bash
yarn install
```

目录结构

```bash
.
├── _config.yml		#站点配置文件
├── package.json	#应用程序的信息
├── scaffolds		#模版文件夹
├── source			#资源文件夹
|   ├── _drafts
|   └── _posts
└── themes			#主题文件夹
```

新建一篇文章

```bash
# 如果标题包含空格的话，请使用引号括起来
hexo new [layout] <title>
# layout文章的布局
```

生成静态文件

```bash
hexo generate
# 简写
hexo g
```

清除缓存文件

```bash
hexo clean
```

启动服务器

```bash
hexo s --debug
```

