# playbook

**文件 zookeeper，为搭建zookeeper集群**

**java。yml 单独安装jdk环境**

**cluster-playbook 集群部署(正在完善)**


目录结构
```
|-- group_vars
|   |-- all
|   |-- flume
|   |-- gateway
|   |-- gm
|   |-- hdfs
|   |-- server
|   |-- spark_scala
|   `-- zk
|-- hosts
|-- roles
|   |-- flume
|   |   |-- tasks
|   |   |   `-- main.yml
|   |   `-- templates
|   |       |-- flume.conf.j2
|   |       `-- flume.j2
|   |-- game-gateway
|   |   |-- files
|   |   |   `-- game
|   |   |-- handlers
|   |   |   `-- main.yml
|   |   |-- tasks
|   |   |   `-- main.yml
|   |   `-- templates
|   |       |-- appContext.xml.j2
|   |       |-- deploy.properties.j2
|   |       |-- log4j.properties.j2
|   |       `-- srun.sh.j2
|   |-- game-server
|   |   |-- files
|   |   |   `-- game
|   |   |-- handlers
|   |   |   `-- main.yml
|   |   |-- tasks
|   |   |   `-- main.yml
|   |   `-- templates
|   |       |-- appContext.xml.j2
|   |       |-- deploy.properties.j2
|   |       |-- dumpjava.j2
|   |       |-- log4j.properties.j2
|   |       `-- srun.sh.j2
|   |-- hdfs
|   |   |-- tasks
|   |   |   |-- hdfs_config.yml
|   |   |   |-- main.yml
|   |   |   `-- ssh_fence.yml
|   |   `-- templates
|   |       |-- core-site.xml.j2
|   |       |-- hadoop-env.sh.j2
|   |       |-- hdfs-site.xml.j2
|   |       |-- mapred-site.xml.j2
|   |       |-- masters.j2
|   |       |-- slaves.j2
|   |       `-- yarn-site.xml.j2
|   |-- jdk
|   |   `-- tasks
|   |       `-- main.yml
|   |-- mount-disk
|   |   `-- tasks
|   |       `-- main.yml
|   |-- mysql-init
|   |   `-- tasks
|   |       `-- main.yml
|   |-- nfs
|   |   `-- templates
|   |       `-- exports.j2
|   |-- ops
|   |   |-- files
|   |   |   `-- Log
|   |   |-- tasks
|   |   |   `-- main.yml
|   |   `-- templates
|   |       `-- clean-redis.j2
|   |-- spark-scala
|   |   |-- tasks
|   |   |   `-- main.yml
|   |   `-- templates
|   |       |-- env.sh.j2
|   |       |-- root.j2
|   |       `-- spark-env.sh.j2
|   |-- tomcat
|   |   |-- files
|   |   |   `-- gm.sql
|   |   |-- tasks
|   |   |   `-- main.yml
|   |   `-- templates
|   |       |-- applicationContext-mybatis.xml.j2
|   |       |-- jdbc.properties.j2
|   |       `-- upgm.j2
|   |-- zabbix-agent
|   |-- zabbix-server
|   |-- zookeeper-alone
|   |   `-- tasks
|   |       `-- main.yml
|   `-- zookeeper-cluster
|       `-- tasks
|           `-- main.yml
|-- site.retry
`-- site.yml
```
