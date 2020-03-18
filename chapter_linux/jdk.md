
tar zxvf xxxx.tar.gz	untar
mv dir1 dir2		rename dir

tar xvJf  node-v8.9.4-linux-x64.tar.xz

3.设置环境变量

[root@localhost java]# vi /etc/profile

在profile中添加如下内容:

#set java environment
JAVA_HOME=/usr/java/jdk1.7.0_79
JRE_HOME=/usr/java/jdk1.7.0_79/jre
CLASS_PATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar:$JRE_HOME/lib
PATH=$PATH:$JAVA_HOME/bin:$JRE_HOME/bin
export JAVA_HOME JRE_HOME CLASS_PATH PATH


让修改生效:

[root@localhost java]# source /etc/profile



test:
java -version
