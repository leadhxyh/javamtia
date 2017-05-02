本项目系《Java多线程编程实战指南（核心篇）》的配套源码。
# 豆瓣主页
https://book.douban.com/subject/27034721/
# 购买链接

# 试读下载
（待补充）
# 内容简介
随着现代处理器的生产工艺从提升处理器主频频率转向多核化，即在一块芯片上集成多个处理器内核（Core），多核处理器（Multicore Processor）离我们越来越近了——如今就连智能手机这样的消费类设备都已配备了4核乃至8核的处理器，更何况商用系统！在此背景下，以往靠单个处理器自身处理能力的提升所带来的软件计算性能提升的那种“免费午餐”已不复存在，这使得多线程编程在充分利用计算资源、提高软件服务质量方面扮演了越来越重要的角色。故而，掌握多线程编程技能对广大开发人员的重要性亦由此可见一斑。《Java多线程编程实战指南（核心篇）》以基本概念、原理与方法为主线，辅以丰富的实战案例和生活化实例，并从Java虚拟机、操作系统和硬件多个层次与角度出发，循序渐进、系统地介绍Java平台下的多线程编程核心技术及相关工具。

《Java多线程编程实战指南（核心篇）》适合有一定Java语言基础的读者作为入门多线程编程之用，也适合有一定多线程编程经验的读者作为重新梳理知识结构以提升认知层次和参考之用。
# 目录
第一部分 多线程编程基础

第1章 走近Java世界中的线程	2

1.1 进程、线程与任务	2

1.2 多线程编程简介	4

1.2.1 什么是多线程编程	4

1.2.2 为什么使用多线程	4

1.3 Java线程API简介	5

1.3.1 线程的创建、启动与运行	5

1.3.2 Runnable接口	9

1.3.3 线程属性	12

1.3.4 Thread类的常用方法	14

1.3.5 Thread类的一些废弃方法	16

1.4 无处不在的线程	17

1.5 线程的层次关系	19

1.6 线程的生命周期状态	21

1.7 线程的监视	22

1.8 多线程编程简单运用实例	26

*1.9 多线程编程的优势和风险	27

1.10 本章小结	29

第2章 多线程编程的目标与挑战	31

2.1 串行、并发与并行	31

2.2 竞态	33

2.2.1 二维表分析法：解释竞态的结果	37

2.2.2 竞态的模式与竞态产生的条件	39

2.3 线程安全性	42

2.4 原子性	43

2.5 可见性	49

2.6 有序性	56

2.6.1 重排序的概念	56

2.6.2 指令重排序	57

2.6.3 存储子系统重排序	63

2.6.4 貌似串行语义	66

2.6.5 保证内存访问的顺序性	68

2.7 上下文切换	69

2.7.1 上下文切换及其产生原因	69

2.7.2 上下文切换的分类及具体诱因	70

2.7.3 上下文切换的开销和测量	71

2.8 线程的活性故障	73

2.9 资源争用与调度	74

2.10 本章小结	77

第3章 Java线程同步机制	80

3.1 线程同步机制简介	80

3.2 锁概述	81

3.2.1 锁的作用	82

3.2.2 与锁相关的几个概念	84

3.2.3 锁的开销及其可能导致的问题	86

3.3 内部锁：synchronized关键字	86

3.4 显式锁：Lock接口	89

3.4.1 显式锁的调度	91

3.4.2 显式锁与内部锁的比较	92

3.4.3 内部锁还是显式锁：锁的选用	95

*3.4.4 改进型锁：读写锁	95

3.5 锁的适用场景	99

3.6 线程同步机制的底层助手：内存屏障	99

*3.7 锁与重排序	102

3.8 轻量级同步机制：volatile关键字	105

3.8.1 volatile的作用	105

3.8.2 volatile变量的开销	111

3.8.3 volatile的典型应用场景与实战案例	111

3.9 实践：正确实现看似简单的单例模式	120

3.10 CAS与原子变量	126

3.10.1 CAS	127

3.10.2 原子操作工具：原子变量类	129

3.11 对象的发布与逸出	135

3.11.1 对象的初始化安全：重访final与static	137

3.11.2 安全发布与逸出	142

3.12 本章小结	143

第4章 牛刀小试：玩转线程	148

4.1 挖掘可并发点	148

4.2 新战场上的老武器：分而治之	148

4.3 基于数据的分割实现并发化	149

4.4 基于任务的分割实现并发化	158

4.4.1 按任务的资源消耗属性分割	159

4.4.2 实战案例的启发	169

4.4.3 按处理步骤分割	171

4.5 合理设置线程数	172

4.5.1 Amdahl's定律	172

4.5.2 线程数设置的原则	173

4.6 本章小结	177

第5章 线程间协作	179

5.1 等待与通知：wait/notify	179

5.1.1 wait/notify的作用与用法	180

5.1.2 wait/notify的开销及问题	188

5.1.3 Object.notify()/notifyAll()的选用	191

*5.1.4 wait/notify与Thread.join()	191

5.2 Java条件变量	192

5.3 倒计时协调器：CountDownLatch	198

5.4 栅栏（CyclicBarrier）	203

5.5 生产者—消费者模式	210

5.5.1 阻塞队列	213

5.5.2 限购：流量控制与信号量（Semaphore）	216

*5.5.3 管道：线程间的直接输出与输入	218

5.5.4 一手交钱，一手交货：双缓冲与Exchanger	221

5.5.5 一个还是一批：产品的粒度	223

5.5.6 再探线程与任务之间的关系	224

5.6 对不起，打扰一下：线程中断机制	225

5.7 线程停止：看似简单，实则不然	228

5.7.1 生产者—消费者模式中的线程停止	233

5.7.2 实践：Web应用中的线程停止	233

5.8 本章小结	236

第6章 保障线程安全的设计技术	240

*6.1 Java运行时存储空间	240

6.2 大公无私：无状态对象	243

6.3 以“不变”应万变：不可变对象	248

6.4 我有我地盘：线程特有对象	254

6.4.1 线程特有对象可能导致的问题及其规避	258

6.4.2 线程特有对象的典型应用场景	264

6.5 装饰器模式	265

6.6 并发集合	267

6.7 本章小结	270

第7章 线程的活性故障	273

7.1 鹬蚌相争：死锁	273

7.1.1 死锁的检测	274

7.1.2 死锁产生的条件与规避	283

7.1.3 死锁的恢复	296

7.2 沉睡不醒的睡美人：锁死	301

7.2.1 信号丢失锁死	301

7.2.2 嵌套监视器锁死	301

7.3 巧妇难为无米之炊：线程饥饿	307

7.4 屡战屡败，屡败屡战：活锁	307

7.5 本章小结	308

第8章 线程管理	310

8.1 线程组	310

8.2 可靠性：线程的未捕获异常与监控	311

8.3 有组织有纪律：线程工厂	316

8.4 线程的暂挂与恢复	318

8.5 线程的高效利用：线程池	320

8.5.1 任务的处理结果、异常处理与取消	326

8.5.2 线程池监控	329

8.5.3 线程池死锁	330

8.5.4 工作者线程的异常终止	330

8.6 本章小结	331

第9章 Java异步编程	333

9.1 同步计算与异步计算	333

9.2 Java Executor框架	336

9.2.1 实用工具类Executors	337

9.2.2 异步任务的批量执行：CompletionService	339

9.3 异步计算助手：FutureTask	344

9.3.1 实践：实现XML文档的异步解析	345

9.3.2 可重复执行的异步任务	349

9.4 计划任务	352

9.5 本章小结	358

第10章 Java多线程程序的调试与测试	360

10.1 多线程程序的调试技巧	360

10.1.1 使用监视点	360

10.1.2 设置暂挂策略	361

10.2 多线程程序的测试	363

10.2.1 可测试性	364

10.2.2 静态检查工具：FindBugs	369

10.2.3 多线程程序的代码复审	370

10.2.4 多线程程序的单元测试：JCStress	372

10.3 本章小结	375

第二部分 多线程编程进阶

第11章 多线程编程的硬件基础与Java内存模型	378

11.1 填补处理器与内存之间的鸿沟：高速缓存	378

11.2 数据世界的交通规则：缓存一致性协议	382

11.3 硬件缓冲区：写缓冲器与无效化队列	386

11.3.1 存储转发	388

11.3.2 再探内存重排序	388

11.3.3 再探可见性	391

11.4 基本内存屏障	392

11.5 Java同步机制与内存屏障	395

11.5.1 volatile关键字的实现	395

11.5.2 synchronized关键字的实现	397

11.5.3 Java虚拟机对内存屏障使用的优化	398

11.5.4 final关键字的实现	398

11.6 Java内存模型	399

11.6.1 什么是Java内存模型	400

11.6.2 happen(s)-before关系	401

11.6.3 再探对象的安全发布	407

11.6.4 JSR 133	411

11.7 共享变量与性能	411

11.8 本章小结	411

第12章 Java多线程程序的性能调校	415

12.1 Java虚拟机对内部锁的优化	415

12.1.1 锁消除	415

12.1.2 锁粗化	417

12.1.3 偏向锁	419

12.1.4 适应性锁	420

12.2 优化对锁的使用	421

12.2.1 锁的开销与锁争用监视	421

12.2.2 使用可参数化锁	424

12.2.3 减小临界区的长度	428

12.2.4 减小锁的粒度	432

12.2.5 考虑锁的替代品	438

12.3 减少系统内耗：上下文切换	438

12.4 多线程编程的“三十六计”：多线程设计模式	440

12.5 性能的隐形杀手：伪共享	441

12.5.1 Java对象内存布局	442

12.5.2 伪共享的侦测与消除	445

12.6 本章小结	454

Web参考资源	457

参考文献	463



