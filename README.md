# pku_hall

1.本应用提供了用户自主查询和定时推送两种方式查询北大百讲当日最新的票务信息，让用户可以随时随地了解最新票务情况。

2.其中index.js文件为被动响应消息，即用户点击菜单发送最新的票务信息。send.js文件为主动群发北大百讲最新票务信息给用户，本应用主动群发给用户的时间为早上9:00.

3.spider.js文件为爬虫文件，每日00:00定时爬取北大百讲官网的最新票务信息，lib目录下的news.js文件则为图文信息的增删改查，本应用推送的图文信息是由每日爬取的票务信息自动生成的图文信息。

# pku_hall
