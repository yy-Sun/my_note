---
title: hexo常用命令
date: 2024-05-03 18:06:17
---

## 创建新文章

```bash
hexo new page --path _posts/about/me "About me"
```

以上命令会创建一个 `me.md` 文件，同时标题为 "About me"

## tag 插件 （keep）

https://v3.keep-docs.xpoet.cn/writing/tag-plugins.html

### note 注解

```
{% note [type] %}
text
{% endnote %}
```

1. `[type]` 设置 note 注解的样式类型
   可选值：`info` | `primary` | `success` | `warning` | `danger`

- 示例：

  ```
  {% note primary %}
  this is primary note ...
  {% endnote %}
  ```

  效果图：![image](data:image/png;base64,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)

- 示例：

  ```
  {% note danger %}
  this is danger note ...
  {% endnote %}
  ```

  效果图：![image](data:image/png;base64,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)

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

生成网页文件并部署至服务器上。

```sh
hexo generate && hexo deploy
```

您可执行下列的其中一个命令，让 Hexo 在生成完毕后自动部署网站，两个命令的作用是相同的。

```sh
$ hexo generate --deploy
$ hexo deploy --generate
```

上面两个命令可以简写为
```sh
$ hexo g -d
$ hexo d -g
```