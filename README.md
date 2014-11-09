hexo-theme-lightup
==================

Hexo theme improved on the basis of [light](https://github.com/hexojs/hexo-theme-light).

# Lightup

基于[Hexo](http://hexo.io/)默认主题改进而来，给你史上最好用的light主题，具体效果见我的博客站点[demo](http://www.seanlook.com)。

## Features
考虑默认google站内搜索大陆地区被墙，
使用见下方

- 集成多说评论功能，增加最新评论widget
- 集成百度分享功能
- 集成swiftype第三方站内搜索，也可以配置使用`wen.lu`
- 集成cnzz站长统计
- 修改归档页的显示，加入所属标签和分类
- 增加返回顶部和文章目录
- 文章详情页加入上下分页
- 文章顶部增加评论数显示
- 加入站点地图（sitemap.xml）和订阅（atom.xml）功能
- 去除多余不使用的功能，如google_analytics和share（twitter无法访问）
- 跳转markdown的最终渲染效果，如引用

- 文章更新日志，有写明`updated: 2014-11-09 00:00:00`的以这个为准，没有显示指定updated将以文件修改时间为准。

如果你需要用回官方addthis，请参照官方light主题。

https://github.com/xiangming/landscape-plus

## Install

执行下面的命令将主题源码下载到您的theme目录，修改站点的`_config.yml`中的`theme`为`lightup`。


```
git clone https://github.com/seanlook/hexo-theme-lightup.git themes/lightup
```

## Config

Default config:

``` yaml
menu:
  Home: /
  Archives: /archives

widgets:
- search
- category
- tag
- twitter

excerpt_link: Read More

twitter:
  username:
  show_replies: false
  tweet_count: 5

addthis:
  enable: true
  pubid:
  facebook: true
  twitter: true
  google: true
  pinterest: true

fancybox: true

google_analytics:
rss:
```

大部分配置请参考官方light主题，下面是需要注意的地方：


- **links** - 友情链接
- **duoshuo_shortname** - 多说评论id
- **baidushare** - 是否开启百度分享
...

## Features

### Gallery Post

![](http://i.minus.com/ibp6Hbytwgof9y.jpg)

```
---
layout: photo
title: Gallery Post
photos:
- http://i.minus.com/ibobbTlfxZgITW.jpg
- http://i.minus.com/iedpg90Y0exFS.jpg
---
```

### Link Post

![](http://i.minus.com/i7hBbGqh14EWo.png)

```
---
layout: link
title: Link Post
link: http://www.google.com/
---
```

### Tweet Widget

![](http://i.minus.com/iMC8EyF9y0Y3y.PNG)

### Fancybox

![](http://i.minus.com/iHv7h7rZNqHvo.PNG)

[Hexo]: http://zespia.tw/hexo/
[AddThis]: https://www.addthis.com
[Fancybox]: http://fancyapps.com/fancybox/
