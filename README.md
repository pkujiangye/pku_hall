# 百讲早知道

## 应用介绍：
    该应用提供了用户自主查询和定时推送(时间为早上9:00)两种方式查询北大百讲当日最新票务信息，让用户可以随时随地了解最新票务情况。

## 系统部署：
    您可以在自己的服务器上测试和使用本应用，但需要具备以下系统环境：
    Node.js >= 0.6.0 npm >= 1.0.0
    
    您需要使用npm工具来获取其它第三方模块支持
    
    本应用采用了回调模式,您需要在微信企业号应用中重新配置服务器。（验证函数verify.js）
    
## 使用说明

    ### 文件结构：
      index.js文件为被动响应消息，即用户点击菜单发送最新票务消息；
      send.js文件为定时主动向用户推送百讲当日最新票务信息;
      spider.js文件为定时爬虫文件，每日00:00准时爬取北大百讲官网的票务信息；
      news.js文件（位于lib目录下）为图文信息增删改查，本应用的图文信息都是由每日爬取的票务信息自动生成的
    
    如需让spider.js和send.js定时启动，index.js能够一直满足点击菜单发送信息，需要将这三个程序一直运行在后台。
    即forever start xx.js，其中node_moudles中已安装了forever模块。

## 开发人员信息
    
    覃浩（1501210392）蒋也（1501210425）

  
