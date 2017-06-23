## ubuntu 安装 MySQL关系型数据库
1. sudo apt-get update 更新源

2. sudo apt-get install mysql-client mysql-server 安装mysql服务器和客户端

3. sudo /etc/init.d/mysqld start 启动mysql服务

## apache安装
1. sudo apt-get update 更新源
2. sudo apt-get install tasksel 安装apache安装包
3. sudo tasksel 启动安装界面
## MySQL 命令行操作
1. 连接Mysql 格式： mysql -h 主机地址 -u用户名 －p用户密码

2. 退出MYSQL命令： exit （回车）

3. 修改密码格式：mysqladmin -u用户名 -p旧密码 password 新密码

4. 创建table的时候就使用utf8编码在每次创建表的时候都在最后加上 character set = utf8 就可以很好的支持中文。
   修改已经有的table的编码,当使用默认编码创建了一个table的时候，是不能支持中文的，这时候使用如下语句对information进行修改：mysql > alter table information convert to character set utf8;

5.  创建数据库：create database <数据库名>

6.  显示数据库：show databases

7.  删除数据库：drop database <数据库名>

8.  使用数据库：use <数据库名>

9.  输出相关信息：select database();

10.  创建数据表：create table <表名>

11.  表结构：desc <表名>

12.  删除表：drop table <表名>

13.  表插入数据：insert into <表名> [( <字段名1>[,..<字段名n > ])] values ( 值1 )[, ( 值n )]

14.  查询表中的数据：select <字段1，字段2，...> from < 表名 > where < 表达式 > 例如：查看表 MyClass 中所有数据 mysql> select *;

15.  修改表中数据：update MyClass set name='Mary' where id=1;

16.  增加字段：alter table 表名 add字段

17.  添加索引：alter table 表名 add index 索引名 (字段名1[，字段名2 ...]);

18.  修改字段：ALTER TABLE table_name ADD field_name field_type;

