Golang
------

参考链接
----

1.  Json <-- [在Golang(GO)中使用JSON——实例解析指南](https://juejin.cn/post/7068173256896806948)
2.  合并map <-- [Go 每日一库之 mergo](https://zhuanlan.zhihu.com/p/112806927)
3.  Mysql <-- [使用GO语言操作MySQL数据库](https://zhuanlan.zhihu.com/p/159266823)，[Golang和MySQL（或PostgreSQL）的使用教程](https://juejin.cn/post/7124915326394826782)，[go操作MySQL](https://topgoer.com/%E6%95%B0%E6%8D%AE%E5%BA%93%E6%93%8D%E4%BD%9C/go%E6%93%8D%E4%BD%9Cmysql/)，[Go 语言操作 MySQL 之 SQLX 包](https://zhuanlan.zhihu.com/p/157480094)
4.  编码处理 <--- [Go-文本编码的转换处理【Transform】【Charset】](https://blog.csdn.net/gaoluhua/article/details/109128154)​[Go-网页编码猜测并转换为UTF-8](https://pkg.go.dev/golang.org/x/net/html/charset)

```text-x-go
reader, err := charset.NewReader(resp.Body, resp.Header.Get("Content-Type"))

func NewReader(r io.Reader, contentType string) (io.Reader, error)
NewReader返回一个io.Reader，它将r的内容转换为UTF-8。它调用DetermineEncoding来找出r的编码是什么。
```

6.  [Go-宝藏](https://www.topgoer.com/)
7.  用 goquery 解析 HTML <-- [zhihu-go 源码解析：用 goquery 解析 HTML](https://liyangliang.me/posts/2016/03/zhihu-go-insight-parsing-html-with-goquery/)
8.  html 选择器示例 <-- [golang goquery selector(选择器) 示例大全](https://cloud.tencent.com/developer/article/1196783)
9.  文件写入 <-- [Golang文件写入的四种方式](https://studygolang.com/articles/29182)
10.  context包 ←- [【Go语言】小白也能看懂的context包详解：从入门到精通](https://segmentfault.com/a/1190000040917752)
11.  userAgent库 ←- [真实设备的userAgent库](https://github.com/zwpro/user-agents)
12.  html-to-markdown ←- [**html-to-markdown**](https://pkg.go.dev/github.com/JohannesKaufmann/html-to-markdown#section-readme)
13.  正则表达式 ←- [【golang】正则表达式 查找和替换字符](https://blog.csdn.net/sphinx1122/article/details/86360427)， [嗨正则](https://hiregex.com/)

‍