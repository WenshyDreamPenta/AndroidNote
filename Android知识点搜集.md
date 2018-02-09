##### 1.LRUCache原理

​	LruCache的核心思想，就是要维护一个缓存对象列表LinkedHashMap，其中对象列表的排列方式是按照访问顺序实现的，即一直没访问的对象，将放在队尾，即将被淘汰。而最近访问的对象将放在队头，最后被淘汰。

​	LruCache中维护了一个集合LinkedHashMap，该LinkedHashMap是以访问顺序排序的。当调用put()方法时，就会在结合中添加元素，并调用trimToSize()判断缓存是否已满，如果满了就用LinkedHashMap的迭代器删除队尾元素，即近期最少访问的元素。当调用get()方法访问缓存对象时，就会调用LinkedHashMap的get()方法获得对应集合元素，同时会更新该元素到队头。

##### 2.图片加载原理

- RGB ：是24位的颜色值，高八位为R，中间八位为G，后八位为B。
  ARGB：是32位的颜色值。高八位为A，次八位为R，再次八位为G，最后八位为B。
- 如果是标准24位图形,1像素使用24位的表示,也就是24bit,换成字节就是3Byte。

##### 3.模块化实现（好处，原因）

代码结构清晰；协同开发；可维护性。

##### 4. JVM

[深入探究JVM | Java的内存区域解析](http://www.sczyh30.com/posts/Java/jvm-memory/)

Java的内存区域主要分为五部分：

- 程序计数器(PC)
- 虚拟机栈(JVM Stack)
- 本地方法栈(Native Method Stack)
- Java 堆内存(Java Heap)
- 方法区(Method Area)

##### 5. 视频加密传输

统计启动时长,标准

如何保持应用的稳定性

ThreadLocal 原理

谈谈classloader

动态布局

热修复,插件化

HashMap源码,SpareArray原理

性能优化,怎么保证应用启动不卡顿

怎么去除重复代码

SP是进程同步的吗?有什么方法做到同步

介绍下SurfView

HashMap实现原理，ConcurrentHashMap 的实现原理

BroadcastReceiver，LocalBroadcastReceiver 区别

Bundle 机制

Handler 机制

android 事件传递机制

线程间 操作 List

App启动流程，从点击桌面开始

动态加载

类加载器

OSGI

Https请求慢的解决办法，DNS，携带数据，直接访问IP

GC回收策略

画出 Android 的大体架构图

描述清点击 Android Studio 的 build 按钮后发生了什么

大体说清一个应用程序安装到手机上时发生了什么；

对 Dalvik、ART 虚拟机有基本的了解；

Android 上的 Inter-Process-Communication 跨进程通信时如何工作的；

App 是如何沙箱化，为什么要这么做；

权限管理系统（底层的权限是如何进行 grant 的）

进程和 Application 的生命周期；

系统启动流程 Zygote进程 –> SystemServer进程 –> 各种系统服务 –> 应用进程

recycleview listview 的区别,性能

排序，快速排序的实现

树：B+树的介绍

图：有向无环图的解释

TCP/UDP的区别

synchronized与Lock的区别

volatile

Java线程池

Java中对象的生命周期

类加载机制

双亲委派模型

Android事件分发机制

MVP模式

RxJava

抽象类和接口的区别

集合 Set实现 Hash 怎么防止碰撞

JVM 内存区域 开线程影响哪块内存

垃圾收集机制 对象创建，新生代与老年代

二叉树 深度遍历与广度遍历

B树、B+树

消息机制

进程调度

进程与线程

死锁

进程状态

JVM内存模型

并发集合了解哪些

ConCurrentHashMap实现

CAS介绍

开启线程的三种方式,run()和start()方法区别

线程池

常用数据结构简介

判断环（猜测应该是链表环）

排序，堆排序实现

链表反转
