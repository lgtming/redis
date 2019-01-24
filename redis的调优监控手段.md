* Redis 2.6 Watchdog 用来诊断Redsi的延迟问题 耗费性能

 config set watchdog-period 500 开启

config set watchdog-period 0 关闭

* monitor 用来监控redis的执行 可以结合liun的管道命令  | grep keys
* 慢查询分析：slowlog-log-slower-than，slowlog-max-len 使用config来设置
* 检查生产上的key分布以及大key，--bigkeys，
* rename-command 禁用一些命令
* 缓存的命中率 (info state 中 有一个keyspace hits misses两个参数)

