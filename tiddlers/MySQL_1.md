* * *

MySQL
-----

参考链接
----

1.  [MySQL教程：MySQL数据库学习宝典](http://c.biancheng.net/mysql/)
2.  [MySQL唯一约束（UNIQUE KEY）](http://c.biancheng.net/view/2445.html)

其他操作
----

1.  连接登录MySQL  
    `mysql -u root -p`​
2.  使用数据库  
    `USE 数据库名;`​

查询操作
----

查询正在使用的数据库  
`SELECT database();`​

显示数据库列表  
`SHOW databases;`​

显示数据库中的数据表  
`SHOW tables;`​

显示数据表结构  
`DESCRIBE [数据库名.]表名;`​  
`desc [数据库名.]表名;`​

查询指定列有多少数据  
`SELECT count(列名) FROM 表名`​

查询指定列中包含指定内容的数据行  
`SELECT * FROM 表名 WHERE 列名 LIKE "指定内容";`​

查询指定列重复项

查看倒数行

​`select * from 库名.表名 order by 列名 desc limit [倒数起始行], 倒数结尾行;`​​

新增操作
----

创建数据库  
`CREATE DATABASE 数据库名;`​

创建表

新增数据

删除操作
----

删除列  
`ALTER TABLE 表名 DROP COLUMN 列名;`​

删除表所有数据

​`DELETE FROM 库名.表名;`​

修改操作
----

进阶操作
----

备份及恢复表

*   创建一个备份表  
    `create table 备份表名 as select * from 原始表名;`​
*   清空原始表中的数据  
    `truncate table 原始表名;`​
*   从备份表中把数据插入到原始表中  
    `insert into 原始表名 select * from 备份表名;`​

查询表索引  
`SHOW index FROM 表名;`​

创建列索引  
`CREATE index 索引名 ON 表名(列名);`​

分析语句执行时长  
`EXPLAIN [SELECT，DELETE，INSERT或UPDATE语句]`​

重置自增序号  
`ALTER TABLE 表名 AUTO_INCREMENT = 0;`​

```text-x-sql
INSERT INTO 数据库名.表名 (列名1, 列名2, ...)
VALUES(数据1, 数据2, ...);
```

```text-x-sql
create table 数据库名.表名 (
    列名1 列类型,
    列名2 列类型,
    ...
);
```

```text-x-sql
SELECT
    列名, COUNT(列名)
FROM
    表名
GROUP BY
    列名
HAVING
    COUNT(列名) > 1;
```