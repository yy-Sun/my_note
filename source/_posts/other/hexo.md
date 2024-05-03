---
title: hexo常用命令
date: 2024-05-03 18:06:17
---

## 创建新文章

```bash
hexo new page --path _posts/about/me "About me"
```

以上命令会创建一个 `me.md` 文件，同时标题为 "About me"

## 设置文章访问密码

[设置文章访问密码](https://keep-docs.xpoet.cn/writing/front-matter.html#设置文章访问密码)

借助 [hexo-blog-encrypt](https://github.com/D0n9X1n/hexo-blog-encrypt) 插件，可以在 Front-Matter 中，单独为某篇文章设置密码。

设置了密码的文章，在文章内容页面会出现密码输入框，只有在输入正确密码后才能阅读文章详情。

使用教程：

1. 安装 hexo-blog-encrypt

   ```sh
   cd your-hexo
   npm install hexo-blog-encrypt
   ```

2. 配置 `password` 属性

   

   ```sh
   ---
   ...
   ...
   password: xxx
   ---
   ```

## 部署到个人服务器

https://www.glimound.com/build-hexo-blog/
