### 概述
#### 1.基本特征
* 并发
并发：并发是指宏观上在**一段时间内能同时运行多个程序**。      
并行：**指同一时刻能运行多个指令**。       
**并行需要硬件支持，如多流水线、多核处理器**或者分布式计算系统。    
**操作系统通过引入进程和线程，使得程序能够并发运行**。      
* 共享
共享：系统中的资源可以被多个并发进程共同使用。    
共享方式：互斥共享和同时共享。   
互斥共享的资源称为临界资源，例如打印机等，在同一时刻只允许一个进程访问，需要用同步机制来实现互斥访问。
* 虚拟
虚拟技术：把一个物理实体转换为多个逻辑实体。    
主要有两种虚拟技术：时(时间)分复用技术和空(空间)分复用技术。     
**时分复用技术：多个进程能在同一个处理器上并发执行，让每个进程轮流占用处理器，每次只执行一小个时间片并快速切换**。      
**空分复用技术：虚拟内存，将物理内存抽象为地址空间，每个进程都有各自的地址空间。**
* 异步：进程不是一次性执行完毕，而是走走停停，以不可知的速度向前推进。