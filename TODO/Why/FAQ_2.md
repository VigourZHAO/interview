区别： 
    1.Memcached存储在缓存中，服务关闭后数据不存储；Redis数据可持久化至硬盘。  -  Redis支持的数据结构较多（字符串、哈希表、链表、集合、有序集合等）
    2.Redis只使用单核、Memcached可以使用多核，数据量大时，Memcached性能较好。
    3.Memcached本身不支持分布式，需要客户端结合分布式算法；Redis偏向于在服务端构建分布式存储。
