# docker-nginx-proxy

# for kintohub
使用方法：

假如你获得的url地址为  https://test.abc.com

代理方式可以使用： `curl -L -X GET 'https://test.abc.com/abc?def=ggg' -H 'Cookie: host=google.com;scheme=https'`

即可访问 https://google.com/abc?def=ggg

## 为何放进cookie？

> 最开始是放在header的，但是尝试了之后发现不行（似乎被kintohub给过滤掉了）

> 于是就只能往cookie里面噻了。没关系，可以做一个对应的client 用于起一个正常的正向代理跑在本地。或者自己封装一个client 给代码fq使用。


## github api

> https://api.github.com => https://proxy.scjtqs.com/githubmatch 

## telegram api

> https://api.telegram.org => https://proxy.scjtqs.com/tgapi