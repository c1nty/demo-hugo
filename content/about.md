---
title: "About"
date: 2018-07-15T18:17:52+08:00
draft: true
---

### Hugo && GitHub Pages

今天用Hugo实现了GitHub Pages，以后可以当笔记本用了，不过还没找到合适的markdown软件，以前一直用印象笔记，现在想归档一些东西，然而一想到格式转换就有点费劲的感觉，慢慢来。

#### 参考文档：

> 安装和使用Hugo: http://www.gohugo.org/

> 托管在 GitHub Pages上: http://www.gohugo.org/doc/tutorials/github-pages-blog/

#### 遇到的问题：

1. 选择好theme准备部署hugo服务器的时候出现`panic: AllThemes not set`错误。

版本问题，新版本的Hugo在`config.toml`中加入`theme="THEME"`即可，其他类型的配置文件同理。

这个错误百度不出来，还是谷歌好用。

> Ref: https://github.com/gohugoio/hugo/issues/4851

2. `hugo -t themename` 部署网站时显示不出文章

`hugo -t Beg --buildDrafts`，加一个`buildDrafts`参数即可。