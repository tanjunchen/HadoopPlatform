# HadoopPlatform
Build a basic hadoop platform

搭建一个简单的伪分布式Hadoop平台 

大致流程：

1：准备相关软件与安装包、安装好linux系统、（此次使用的是Ubuntu16.04）创建hadoop用户。

2：登录Hadoop用户、安装nanao或vim或vi、更改软件更新源。

3：安装SSH、安装XShell或secureCRT实现远程控制。

4：安装JDK 配置JAVA_HOME环境变量。

5：安装Hadoop 解压hadoop安装包。

6：Hadoop默认是非分布式的 修改相应的配置文件

如core-site.xml、hdfs-site.xml等 这次搭建的是伪分布式平台所以修改上述两个配置文件即可。

7：开启Hadoop 使用。./bin/hdfs namenode -format Exiting with status : 0 表示成功开启。

使用JPS查看是否打开成功 使用JPS后会出现 Jps DataNode SecondaryNameNode FSShell NameNode等

8：启动成功后 可以访问Web界面查看相关信息如  ip地址:50070

9：添加Path路径 因为上述操作都要用到hadoop命令 使用系统命令方便操作
