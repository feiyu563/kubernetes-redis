K8S REDIS 主从模式集群
redis master负责写,slave负责读取.
有状态部署,数据持久化.

先要创建出pool池和storageclass

部署redis集群

kubectl create -f .


端口均采用NodePort,可以自己修改

zxbk-redis-public-read 39557
zxbk-redis-public-write 45730