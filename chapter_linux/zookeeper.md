



To start ZooKeeper you need a configuration file. Here is a sample, create it in conf/zoo.cfg:

tickTime=2000
dataDir=/var/zookeeper
clientPort=2181



bin/zkServer.sh start


>zoo.cfg
server.1=192.168.1.201:2888:3888
server.2=192.168.1.202:2888:3888
server.3=192.168.1.203:2888:3888



echo '1' > data/myid


¹Ø±Õ·À»ðÇ½·½·¨£º sudo service iptables stop


sick:
1.after restart system after stoping firewall. 
2.It show you that the status is ok after you start all zookeepers.



client command
1. start client;
./zkCli.sh

create node
create /root root.vale
set /root new.value
delete /root 
ls /	show nodes under /	
connet ip:port	connet which host you want.
