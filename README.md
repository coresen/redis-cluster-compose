``` shell
# 需在docker-compose.yml所在的文件夹下执行
docker-compose up -d 

# 集群模式
docker exec -it node-80 redis-cli -p 6380 --cluster create 172.16.238.10:6380 172.16.238.11:6381 172.16.238.12:6382 172.16.238.13:6383 172.16.238.14:6384 172.16.238.15:6385 --cluster-replicas 1
```
