SQLyog连接mysql失败问题

😃**DepressiveStar#2**

​     **2020.02.12**



为了方便安装查看，下载sqlyog 工具 连接 mysql

配置新连接报错：错误号码 2058，分析是 mysql 密码加密方法变了。

解决方法：windows 下cmd 登录 mysql -u root -p 登录你的 mysql 数据库，然后 执行这条SQL：

 ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';

#password 是你自己设置的root密码

然后在重新配置SQLyog的连接，则可连接成功了，OK。
