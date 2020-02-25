---
layout: post
title: Google指令--Google搜索
tags: Google
---
想要更高效的使用Google，需要输入三项内容:<br/>
1.你想要用到的指令。<br/>
2.半角冒号(:)。<br/>
3.指令中要用到的具体的内容。<br/>
输入这三项内容后，接下来就跟普通搜索没什么两样了，比如使用“site:”指令，在Google搜索框中输入:
```
#site:domain term(s) to search
#比如
site:bingnaive.github.io
```
这样你搜集到的信息就全部出自baidu.com这个网站中了，使用这个指令可以避免搜索到一大堆不管有用没用的内容，将注意力放到有用的搜索结果上。<br/>
另外还有“intitle”和“allintitle”指令，在搜索框加入这两条指令的话，只有当网页标题中包含你搜索的关键字是，才会出现在搜索结果里。“intitle”和“allintitle”区别是，“allintitle”表示网页标题必须包含所有关键字才会出现在结果里，而“intitle”不用全部，只要包含任意一个关键字即可。<br/>
如果想搜索包含某些特定字符的网站，可以使用“inurl:”指令。比如：
```
#可以发现很多有意思的网站
inurl:admin
```
使用“cache:”指令可以让Google只显示网页快照里的信息
```
cache:bingnaive.github.io
```
“filetype:”指令可以查找扩展名为doc,xlsx,ppt,txt等类型的文件，而且可以多个指令搭配使用。比如
```
site:baidu.com filetype:pptx
```
```
inurl:login
#或者
logon,Signin,Signon,Forgotpassword,Forgot,Reset
```

