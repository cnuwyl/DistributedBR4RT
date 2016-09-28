# DistributedBR4RT
Distributed Balance Routing for Realtime Traffic


这是一个用Storm框架编写的一个北京市交通路况挖掘程序，本程序的功能主要实现的是根据实时gps点的信息进行道路匹配，通过某段道路的所有出租车的平均速度来计算该路段的路况情况。

运行环境：

1. 系统：ubuntu14.04

2. Java环境：jkd1.7

3. 数据库：Postgresql 9.4

4. 编程语言：Java

5. 编程框架： Storm

6. 分布式模式：本地模式

7. 依赖包： Storm_lib, Hdfs_lib, Postgreal_lib, Phonenix_lib

8. 开源地图OpenStreetMap：Beijing.osm

9. gps数据：北京市2010年的某个时段的数据：valid_gps_utc;


注意：

1. 安装Ubuntu，JDK1.7，安装过程可参考网上的安装步骤

2. 先安装postgresql数据库，安装9.4以后的版本，安装过程参考我更新过后的張禹的github,链接：https://github.com/cnuwyl/BalanceRouting4RealtimeTraffic/blob/master/wylong/

3. 安装Storm分布式集群，本地模式下其实只需解压导入依赖包就可以开发了



本程序存在的一些不足：

1. 计算效率不是很好，希望有感兴趣的朋友可以与我们交流和改进

2. 我们的业务逻辑还比较简单，只是进行了地图匹配以及道路车辆速度的计算，并没有做过多的功能性的扩展，欢迎后续的朋友们进行扩展

3. 我们对于任务的分配和设计还不是很合理，这一点可能是影响性能的瓶颈点之一，后续的人员可以从任务与线程分配，接口的合理选择，计算资源扩展等进行改进。
