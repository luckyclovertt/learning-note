# redis
## redis的作用
Redis具有内置复制，Lua脚本，LRU驱逐，事务和不同级别的磁盘持久性，并通过Redis Sentinel提供高可用性，并通过Redis Cluster进行自动分区
## redis命令
1. redis-cli 进入redis数据库
2. set key value   创建一个键值对
3. get key   返回key对应的value
4. mset key1 value1 key2 value2  创建多个键值对
5. mget key1 key2 返回多个value
6. sadd key value  创建集合
7. smembers key 集合中key对应的value
## flask使用redis
    import redis   引入redis
    rdb = redis.(Strict)Redis(host='localhost',port=6379,db=0)  
    rdb.mset(key1='value1',key2='value2'...)    
    rdb.get('key1')
    

