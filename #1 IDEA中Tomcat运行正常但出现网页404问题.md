## IDEA中Tomcat运行正常但出现网页404问题
😃**DepressiveStar#1**

​     **2020.02.12**

今天在IDEA中创建maven项目，部署完Tomcat配置，测试项目，打开网页出现404问题

![](C:\Users\DepressiveStar\Desktop\404.png)

在经过一上午抓狂的百度后，发现问题出在ProjectStructure中

![](C:\Users\DepressiveStar\Desktop\module错误.png)

原因在于Web中两个路径不是main中的webapp文件夹

更改后结果如下

![](C:\Users\DepressiveStar\Desktop\module更正.png)

运行测试

![](C:\Users\DepressiveStar\Desktop\显示成功.png)

结果成功

