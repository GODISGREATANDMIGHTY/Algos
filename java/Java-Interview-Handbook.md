# 📘 Java 完整面试手册（Java Interview Handbook）

> 覆盖：基础 → 进阶 → 并发 → JVM → 框架 → 分布式 → 高并发 → 架构设计 → 生产运维  
> 定位：面试宝典 + 技术体系 + 架构思维 + 工程能力  
> 适用人群：Java 后端工程师 / 高级工程师 / 架构师 / 分布式系统工程师

---

# 📑 目录（Contents）

1. Java 基础
2. 面向对象（OOP）
3. Java 集合框架
4. 异常体系
5. Java IO / NIO / AIO
6. Java 并发编程
7. 线程与线程池
8. 锁机制与并发控制
9. 并发容器
10. JVM 虚拟机
11. JVM 调优
12. 类加载机制
13. 反射 & 动态代理
14. 注解机制
15. 设计模式
16. Spring 核心
17. Spring MVC
18. Spring Boot
19. Spring Cloud / 微服务
20. MyBatis / ORM
21. 数据库基础
22. MySQL 深入
23. Redis
24. 消息队列 MQ
25. 分布式系统
26. 高并发系统设计
27. 高可用架构
28. 缓存架构
29. 分布式事务
30. 系统设计题
31. 架构设计题
32. DevOps / 运维
33. 云原生
34. Kubernetes
35. 生产级场景题
36. 架构表达类面试题

---

# 第一章 Java 基础

- Java 特性
- JDK / JRE / JVM 区别
- Java 编译与运行流程
- 基本数据类型
- 包装类型
- 自动装箱拆箱
- == vs equals
- hashCode 作用
- String / StringBuilder / StringBuffer
- final / finally / finalize
- static 关键字
- this / super
- 深拷贝 vs 浅拷贝

---

# 第二章 面向对象（OOP）

- 封装
- 继承
- 多态
- 抽象类 vs 接口
- 接口 default 方法
- 组合 vs 继承
- 面向接口编程思想
- 依赖倒置原则
- 单一职责原则
- 开闭原则
- 里氏替换原则

---

# 第三章 集合框架

- Collection vs Map
- List / Set / Map 体系结构
- ArrayList 原理
- LinkedList 原理
- HashMap 原理
- HashSet 原理
- TreeMap 原理
- ConcurrentHashMap 原理
- fail-fast 机制
- fail-safe 机制

---

# 第四章 异常体系

- Error vs Exception
- Checked vs Unchecked
- try-catch-finally
- throws vs throw
- 自定义异常
- 全局异常处理机制
- 异常设计规范

---

# 第五章 IO / NIO / AIO

- BIO 模型
- NIO 模型
- AIO 模型
- Reactor 模型
- Proactor 模型
- 零拷贝
- Netty 模型

---

# 第六章 Java 并发编程

- 并发 vs 并行
- 进程 vs 线程
- 并发三大特性
  - 原子性
  - 可见性
  - 有序性
- JMM 内存模型
- happens-before
- volatile
- 指令重排
- 内存屏障

---

# 第七章 线程与线程池

- 线程创建方式
- Runnable vs Callable
- Future vs CompletableFuture
- 线程生命周期
- 守护线程
- ThreadPoolExecutor
- 线程池参数
- 线程池执行流程
- 线程池设计公式
- CPU 密集型配置
- IO 密集型配置
- 线程池拒绝策略
- 线程池高可用设计
- 线程池 OOM

---

# 第八章 锁机制

- synchronized 原理
- 锁升级过程
- 偏向锁
- 轻量级锁
- 重量级锁
- ReentrantLock
- 公平锁 / 非公平锁
- 乐观锁 / 悲观锁
- CAS
- ABA 问题
- 自旋锁
- 死锁
- 活锁
- 饥饿问题

---

# 第九章 并发容器

- ConcurrentHashMap
- CopyOnWriteArrayList
- BlockingQueue
- DelayQueue
- SynchronousQueue

---

# 第十章 JVM

- JVM 架构
- 内存模型
- 运行时数据区
- 栈 / 堆 / 方法区
- 程序计数器
- GC Roots
- 对象创建过程
- 对象内存布局

---

# 第十一章 JVM 调优

- GC 算法
- CMS
- G1
- ZGC
- GC 调优思路
- OOM 排查
- 内存泄漏排查
- jmap / jstack / jstat
- Arthas

---

# 第十二章 类加载机制

- 类加载过程
- 双亲委派模型
- 类加载器
- 热加载
- SPI 机制

---

# 第十三章 反射 & 动态代理

- 反射原理
- JDK 动态代理
- CGLIB 动态代理
- AOP 原理

---

# 第十四章 注解

- 注解原理
- 元注解
- 自定义注解
- 注解解析

---

# 第十五章 设计模式

- 单例
- 工厂
- 建造者
- 代理
- 策略
- 模板方法
- 责任链
- 观察者
- 适配器
- 装饰器

---

# 第十六章 Spring

- IOC
- DI
- Bean 生命周期
- Bean 作用域
- AOP
- 事务机制
- 事务传播机制
- 事务失效场景

---

# 第十七章 Spring MVC

- DispatcherServlet
- 请求流程
- 拦截器
- 参数绑定
- 视图解析器

---

# 第十八章 Spring Boot

- 自动装配原理
- starter 原理
- SPI 机制
- 配置加载顺序

---

# 第十九章 微服务

- 服务注册发现
- 服务治理
- 服务熔断
- 服务降级
- 服务限流
- 链路追踪
- 灰度发布
- 蓝绿部署
- 金丝雀发布

---

# 第二十章 MyBatis

- 执行流程
- 一级缓存
- 二级缓存
- SQL 映射原理
- 插件机制

---

# 第二十一章 数据库基础

- ACID
- 事务隔离级别
- MVCC
- 锁机制
- 索引结构
- B+Tree

---

# 第二十二章 MySQL 深入

- InnoDB 架构
- redo log
- undo log
- binlog
- 慢查询优化
- 索引优化
- 执行计划

---

# 第二十三章 Redis

- 数据结构
- 持久化机制
- 主从复制
- 哨兵机制
- 集群模式
- 缓存问题
  - 穿透
  - 击穿
  - 雪崩

---

# 第二十四章 MQ

- Kafka
- RabbitMQ
- RocketMQ
- 削峰填谷
- 解耦
- 异步化
- 消息可靠性
- 消息顺序性
- 幂等性
- 事务消息

---

# 第二十五章 分布式系统

- CAP 定理
- BASE 理论
- 一致性模型
- 分布式锁
- 分布式 ID
- 注册中心
- 配置中心

---

# 第二十六章 高并发系统设计

- 削峰
- 限流
- 缓存
- 异步
- 解耦
- 隔离
- 分片
- 负载均衡

---

# 第二十七章 高可用架构

- 冗余设计
- 故障转移
- 自动恢复
- 多活架构
- 异地多活
- 两地三中心
- 脑裂问题

---

# 第二十八章 缓存架构

- 多级缓存
- 本地缓存
- 分布式缓存
- 一致性模型
- 双写一致性
- 延迟双删

---

# 第二十九章 分布式事务

- 2PC
- TCC
- Saga
- 本地消息表
- MQ 事务消息
- 幂等设计

---

# 第三十章 系统设计题

- 秒杀系统
- 订单系统
- 支付系统
- IM 系统
- 日志系统
- 推荐系统
- 短链系统
- 抢票系统

---

# 第三十一章 架构设计题

- 高并发架构设计
- 高可用架构设计
- 分布式架构设计
- 微服务架构设计
- 中台架构设计
- 平台化架构设计

---

# 第三十二章 DevOps

- CI/CD
- 自动化部署
- 自动化测试
- 自动化运维
- 蓝绿发布
- 灰度发布

---

# 第三十三章 云原生

- Docker
- Kubernetes
- Service Mesh
- Istio
- 云原生架构

---

# 第三十四章 Kubernetes

- Pod
- Service
- Deployment
- Ingress
- ConfigMap
- Secret
- HPA
- Operator

---

# 第三十五章 生产级场景题

- 数据库宕机
- Redis 宕机
- MQ 宕机
- 网关挂了
- 配置中心挂了
- 注册中心挂了
- 流量洪峰
- 热点 Key

---

# 第三十六章 架构表达类面试题

- 如何做容量规划？
- 如何做系统治理？
- 如何做服务隔离？
- 如何实现系统自治？
- 如何实现 99.99% 可用性？
- 如何做系统可观测性？
- 如何设计弹性架构？

---

# 📌 项目说明

本项目目标：
- 构建完整 Java 技术体系
- 形成工程级技术能力模型
- 建立架构级系统设计思维
- 支撑中高级技术面试
- 构建长期技术成长路线

关键词：
Java / JVM / 并发 / 分布式 / 高并发 / 高可用 / 架构 / 微服务 / 系统设计