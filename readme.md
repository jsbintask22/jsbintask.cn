# Blog
本博客使用github page和[spfk-j](https://github.com/jsbintask22/hexo-theme-spfk-j.git)主题搭建，该主题是再spfk的基础上进行修改，修改了部分ui，加入了一些新东西，如集成畅言插件等。
![demo](https://raw.githubusercontent.com/jsbintask22/static/master/spfk-j/demo1.png)
![demo](https://raw.githubusercontent.com/jsbintask22/static/master/spfk-j/demo2.png)
![demo](https://raw.githubusercontent.com/jsbintask22/static/master/spfk-j/demo3.png)

# 主题
拉取:
```bash
$ git clone https://github.com/jsbintask22/hexo-theme-spfk-j.git themes/spfk-j
```
## 配置
修改hexo根目录下的 `_config.yml` ： `theme: spfk-j`

## 更新
```bash
cd themes/spfk-j
git pull
```

## 主题配置
```yaml
# >>> Basic Setup | 基础设置 <<<

# Header | 主菜单
## About Page: `hexo new page about`
## Tags Cloud Page: `hexo new page tags`
menu:
  所有标签: /tags
  推荐阅读: /categories/recommend
  光影之路: /instagram
  文章归档: /archives

# Link to your avatar | 填写头像地址
avatar: img/head.jpg

# Small icon of Your site | 站点小图标地址
favicon: img/favicon.png

# Social info. Bar | 社交信息展示
subnav:
  mail: "mailto://jsbintask@gmail.com"
  github: "https://github.com/jsbintask22"
  stackoverflow: "https://stackoverflow.com/users/10720862/jasonzou"
  Instagram: "https://www.instagram.com/jsbintask/"
  # zhihu: "#"
  # weibo: "#"
  # google: "jsbintask@gmail.com"
  # twitter: "#"
  # linkedin: "#"
  # facebook: "#"
  # rss: /atom.xml
  # pinterest: "#"
  # QQ: "1484432123"
  # wechat: "wechat://A1484432123"
  # douban: "#"
  # pinboard: "#"
  # segmentfault: "#"

# >>> Conments 评论系统 <<<
disqus:
  # on: true
  shortname: jsbintask
  # https://help.disqus.com/customer/en/portal/articles/466208-what-s-a-shortname-
  # It is unnecessary to enable disqus here if
  # you have set "disqus_shortname" in your site's "_config.yml"

duoshuo:
  # on: true
  domain: jsbintask
  # 是否开启多说评论，http://duoshuo.com/create-site/
  # 使用上面网址登陆你的多说，然后创建站点，在 domain 中填入你设定的域名前半部分
  # http://<要填的部分>.duoshuo.com (domain只填上<>里的内容，不要填整个网址)

gitment:
  # on:
  owner: jsbintask22
  repo: jsbintask22.gitment.io
  client_id: dab248f1d00073a66261
  client_secret: 944b58055daec75b1cb681cc860f34afac2b9e73

  # 畅言配置，主要去畅言官网注册 http://changyan.kuaizhan.com/，获取相应的appId和conf
  # 注意，除了此处外，每个md文件中还应加入 sourceId，用以唯一标识某篇文章，如没加，也将不会进行评论渲染
changyan:
  on: true
  appId: cyu0pbbdV
  conf: prod_63c6b3d3f6f2019a79293cbf63760587

youyan:
  #on: true
  id:
  # 是否开启友言评论，http://www.uyan.cc/index.php
  # id 中填写你的友言用户数字ID，注册后进入后台管理即可查看
  # 友言服务在 Web 环境下运行，普通本地环境无法查看，请部署后在线上测试。


# >>> Style Customisation 样式自定义 <<<

# Background | 背景
## "background_sum": show images form /source/background/的图片数目
## "on: true": 自动随机显示这5张图片
## "on: false": 自定义显示图片设置background_image: 5
background:
  on: true
  #on: false
  background_sum: 24
  background_image: 109

highlight_style:
  on: true
  inline_code: 5
  code_block: 5
  # 通过 inline_code 切换内置文本高亮样式 Value: 0 - 9 可选
  # 通过 code_block 切换内置代码高亮配色主题  Value: 0 - 4

blockquote_style:
  #on: true
  blockquote: 1  # Value: 0 - 7 可选
  # 自定义文章「引用部分」的样式

# 左边栏宽度 px
left_col_width: 300

# 目录中标题不换行
# Keep TOC title on the same line |
toc_nowrap: false

# 自定义"阅读全文"链接按钮的显示文字
# Customize the text on excerpt link
excerpt_link: 阅读全文

# 是否显示边栏中的搜索框（仅样式，未添加搜索功能）
# Search Box in left column
# search_box: true

# 是否开启主页及加载头像时的动画效果
# Animation in Homepage and Loading avatar
animate: true


# >>> Small features | 小功能设置 <<<

# 是否开启边栏多标签切换
# Birdhouse button in left column
tagcloud: true

# Blogroll, Link exchange | 友情链接
# friends: false
friends:
  gayhub: https://github.com

# 打赏
# 请在需要打赏的文章的md文件头部，设置属性reward: true

# 打赏基础设定：0-关闭打赏； 1-文章对应的md文件里有reward:true属性，才有打赏； 2-所有文章均有打赏
reward_type: 2
# 打赏wording
reward_wording1: '谢谢你支持我分享知识'
reward_wording2: '扫码打赏，心意已收'
# 支付宝二维码图片地址，跟你设置头像的方式一样。比如：/img/alipay.jpg
#alipay: /img/alipay.png
# 微信二维码图片地址
weixin: /img/weixin.png

#是否开启“关于我”。
aboutme: 96年，java工程师，爱折腾！
#aboutme: false

# 是否在新窗口打开链接
# Open ALL link in a new tab
open_in_new: false

# Customize feed link 自定义订阅地址
rss: /atom.xml


# >>> Vendors | 第三方工具 & 服务 <<<

# images viewer | 图片浏览器
## http://www.fancyapps.com/fancybox/
fancybox: true

# Display Math(LaTeX, MathML...) | 数学公式支持
## https://www.mathjax.org/
mathjax: true

# Socail Share | 是否开启分享
# share: true
baidushare: true
#showshare: true

# 百度、谷歌站长验证。填写 HTML 标签 content
# Site Verification for Google and Baidu. HTML label content.
google_site: # pFW527fHrjfI0si2w4NQ0w3cTw12AvvuohAu1PUfqKA
baidu_site: #c167b9feb4f0b208b712c79629c188e4

# Fill in Google Analytics tracking ID, #e.g. UA-XXXXX-X, or Baidu Analytics hash key
google_analytics:
baidu_analytics: f1c1bcd43bb13500d087f18deb22025f

# 不蒜子网站计数设置
# http://ibruce.info/2015/04/04/busuanzi/
visit_counter:
  on: true
  site_visit: 本站访问量
  page_visit: 本文阅读量

# A标签提示
TipTitle: true

# Loading
Loading: true

# 是否显示二维码名片，此处的路径是 spfk下source 里面的路径
qrcodePath: /img/wechat_public.jpg
```

**另外欢迎fork和star，如果搭建过程有问题，可随时和作者联系 jsbintask@foxmail.com**