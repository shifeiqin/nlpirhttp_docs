# 搜索相关接口说明

**1.搜索接口使用说明**

`URL：`[`http://127.0.0.1:8080/NLPIR_HTTP/HttpJZSearch`](http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas)

`参数：content,start,pageCount,ip,port`

```
    参数依次代表：搜索命令（如：[cmd] list all）、记录起始号、一页查询记录条数、搜索服务IP、搜索服务端口PORT
```

`return：String     返回字符串，`

`<?xml version="1.0" encoding="utf-8" standalone="yes" ?>`

`<JZSearch-Result>`

`    <Result-Number>`

`        <Total-Number>35427</Total-Number>`

`        <Return-Number>1</Return-Number>`

`        <Start-Position>0</Start-Position>`

`    </Result-Number>`

`    <Result>`

`        <Document>`

`            <doc_id>0</doc_id>`

`            <score>0.00</score>`

`            <id>2</id>`

`            <title>《改革世贸组织：多哈回合中的发展中成员》出版</title>`

`            <content>中新网上海11月20日电(记者 邹瑞玥)20日，由WTO事务咨询中心成员翻译、上海人民出版社出版的《改革世界贸易组织：多哈回合中的发展中成员》在沪举行新书发布会。全书约20万字，为评估WTO中那些更为强大的发展中成员集团的作用提供了一个概念性框架。&#x0D;多哈回合谈判于2001年11月启动，按计划应在2005年1月1日前结束。但因</content>`

`            <published_at>2011/11/21 11:01:00</published_at>`

`            <active>1</active>`

`        </Document>`

`    </Result>`

`</JZSearch-Result>`

