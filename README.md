# coney
based on [Pacman](https://github.com/A-limon/pacman).

coney is a flat and responsive design theme for [Hexo](http://hexo.io).

you can star my porject to get information while I update the theme.

[Demo](http://gengbiao.me)

中文说明地址点[这里](http://gengbiao.me/2014/10/13/coney%E4%B8%BB%E9%A2%98%E4%BB%8B%E7%BB%8D/)

##Installation
###Install
```
$ git clone -b master https://github.com/coneycode/coney-hexo-theme
```
**Coney requires Hexo 2.4.5 and above.** 
###Enable
Modify `theme` setting in blog folder` _config.yml` to `coney`.
```
theme = coney
```
###Update
```
cd themes/coney-hexo-theme
git pull
```

**please backup your `_config.yml` file before update.** 
##Configuration

Modify settings in  `/themes/coney/_config.yml`.
```yml
##### Menu
menu:
  Home: /
  Archives: /archives
## you can create `tags` and `categories` folders in `../source`.
## And create a `index.md` file in each of them.
## set `front-matter`as
## layout: tags (or categories)
## title: tags (or categories)
## ---

#### Widgets
widgets: 
- category
- tag
- links
- rss
- tagcloud
## provide six widgets:category,tag,rss,archive,tagcloud,links.
## modify links in `/layout/_widget/links.ejs`.

#### RSS
rss:  atom.xml ## RSS address.

#### Image
imglogo:
  enable: false             ## display image logo true/false.
  src: img/logo.svg        ## `.svg` and `.png` are recommended,please put image into the theme folder `/coney/source/img`.

favicon: img/favicon.ico   ## size:32px*32px,`.ico` is recommended,please put image into the theme folder `/coney/source/img`.     

#### Author Avatar Picture
author_img_enable: true ## display author avatar picture
author_img: img/coney.png ## size:220px*220px.
## if the picture's format is `.png` or `.jpg`  instead of dataURI,you should set the `dataURI` value to false.

#### Font
ShowCustomFont: true  
## you can change custom font in `variable.styl` and `font.styl` which in the theme folder `/coney/source/css`.

#### Toc
toc:
  article: true   ## show contents in article.
  aside: true     ## show contents in aside.
## you can set both of the value to true of neither of them.
## if you don't want display contents in a specified post,you can modify `front-matter` and add `toc: false`.

#### Fancybox
fancybox: false 
## if you use gallery post or want use fancybox please set the value to true.
## if you want use fancybox in ANY post please copy the file `fancybox.js`.
## in theme folder `/coney/scripts` to your hexo blog folder `../scritps`.

#### Author information
author:
  google_plus:    ## eg:116338260303228776998 for https://plus.google.com/u/0/116338260303228776998
  weibo:      coneylife ## e.g. 436062867 for http://weibo.com/436062867
  twitter:    ## e.g. gengbiaosky for https://twitter.com/yangjiansky
  github:     coneycode ## e.g. coneycode for https://github.com/coneycode
  facebook:   ## e.g. gengbiao for https://favebook.com/yangjian
  tsina:      1005055274569156 ## e.g. 1664838973  Your weibo ID,It will be used in share button.
  zhihu:     # coneylife, now it is no icon, I have push an issue to Font Awesome.

#### Comment
duoshuo: 
  enable: true  ## duoshuo.com
  short_name: coney ## duoshuo short name.

#### Share button
jiathis:
  enable: false ## if you use jiathis as your share tool,the built-in share tool won't be display.
  id:    ## e.g. 1501277 your jiathis ID. 
  tsina: ## e.g. 1664838973 Your weibo id,It will be used in share button.

####Baidu Analytics
baidu_analytics:
  enable: true
  id: # your baidu analytics id
####Baidu Share
baidu_share:
  enable: true
baidu_search:
  enable: true
  id:   #your baidu_search_id
  site: http://search.baidu.com/cse/search  #your can change your site instead the default site
google_analytics:
  enable: true
  id:   ## e.g. UA-55273525-1  your google analytics ID.
  site: gengbiao.me ## e.g. gengbiao.me your google analytics site or set the value as auto.
## You MUST upgrade to Universal Analytics first!
## https://developers.google.com/analytics/devguides/collection/upgrade/?hl=zh_CN

####background music 
background_music:
  enable: false
  src: 
#### Custom Search
google_cse: 
  enable: false
  cx:  ## e.g. 000561263943549425496:91c2z8qybp0 your Custom Search ID
## https://www.google.com/cse/ 
## To enable the custom search You must create a "search" folder in '/source' and a "index.md" file
## set the 'front-matter' as
## layout: search 
## title: search
## ---


```
