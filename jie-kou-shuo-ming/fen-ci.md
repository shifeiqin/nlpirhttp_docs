# 分词相关接口说明

**1.字符串分词接口**

`URL：`[`http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas`](http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas)

`参数：content,type`

`return：String`

例：_面贴/nvercat    一下/mq    解/v    薄弱测试/nvercat    决/vg    这个/rz    奥巴马/AWK    问题/n    参考/vn    字符转码/user    的/ude1    文章/n    小尾羊/nvercat    大/a    尾/q    羊/n_

**2.新增单词接口**_    _

`URL：`[`http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclasAddUserWord`](http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas)

`参数：content       用户词，格式“词 词性”，词和词性以空格分开的字符串。`

`return：true or false;`

_**调用该接口，将会向分词系统导入一个用户词，如果是临时使用，那么指定用该接口，系统只是加载到分词系统的内存中，如系统推出，重加初始化使用，那么添加的词将不再起作用。**_

**3.保存单词接口**_**   ** _

`URL：`[`http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclasSaveUserWord`](http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas)

`return：true or false;`

_**为了保证单词添加接口添加的词长期有效，那么需要调用用户词保存接口。**_

_**保存后下次分词系统初始化后无需重复导入用户词即可使用。**_

**4.删除单词接口**_**    **_

`URL：`[`http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclasDelUserWord`](http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas)

`参数：content       要删除的用户词。词语字符串`

`return：true or false;`

**5.导入文件接口**_**    **_

`URL：`[`http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclasImpUserDict`](http://127.0.0.1:8080/NLPIR_HTTP/HttpIctclas)

`参数：path   文件路径`

`type   是否覆盖现有用户词典，1为覆盖，0为不覆盖。`

`return：导入的次数`

