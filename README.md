## Nanboone
a ghost theme inspired by [TryGhost/Casper](https://github.com/TryGhost/Casper) and [TryGhost/Blog](https://github.com/TryGhost/Blog).          
一个大图大字体的Ghost主题

## [Live Demo ](https://cjupup.github.io/demo/nanboone/)



## 一. 安装主题

1. 点击[这里](https://github.com/cjupup/ghost-theme-nanboone/releases)下载主题压缩包

2. 进入自己的Ghost博客后台，点击：SETTINGS->Design->Upload a theme，上传第一步下载的主题包并启用主题

  



## 二. 自定义主题  

#### 本地安装 Ghost

详细安装步骤请参见 [How to install Ghost locally](https://ghost.org/docs/setup/)

本地安装 Ghost 完成后，进入 Ghost 根目录，运行下面命令启动 Ghost：

```
ghost start
```

终端输出如下信息

```
➜  GhostLocal ghost start
✔ Checking current folder permissions
✔ Validating config
✔ Checking memory availability
✔ Starting Ghost

------------------------------------------------------------------------------

Your admin interface is located at: 

    http://localhost:2368/ghost/
```

打开 `http://localhost:2368/ghost/`，进入 Ghost 后台。

#### 启用主题

下载主题 zip 压缩包，进入本地启动的 Ghost 博客后台，点击：SETTINGS->Design->Upload a theme，上传下载的主题包，`active theme`。

#### 2.1 修改默认样式  

终端`cd` 命令进入`content/themes/nanboone`目录，`yarn install`安装依赖包，安装完成后，运行`yarn run dev` 。

修改主题的样式源文件（位于`/res/css/` 目录），它们将自动编译到 `/assets/css/`目录，即可定义自己喜欢的样式，本地浏览器刷新 `http://localhost:2368` 可以查看修改后的网站样式。   

最后，将`/assets/css/` 目录的文件上传到自己服务器上即可。

#### 2.2 添加评论   

主题默认使用 Disqus 评论系统，注册 Disqus 后将你的 shortname 填入 `partials/comments.hbs` 下面的位置即可：

```
var disqus_shortname = '你的 Disqus shortname';
```

#### 2.3 添加归档页

可参考[这篇文章](https://yehuzi.com/gei-ghostbo-ke-tian-jia-tagsgui-dang-ye/)

#### 2.4 国际化    

目前提供了三个版本的语言（简体/英文/繁体）。启用步骤：登录管理后台，选择 `Setting/General`，在 `Publication Language` 文本框内输入任意(zh-CN/en/zh-TW)后保存即可。     


## 三. 截图 
  
![](/nanbooness.42f27df9.jpg)    
