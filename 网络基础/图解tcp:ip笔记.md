[TOC]



### 第1章 网络基础知识

#### 1.5协议分层与OSI参考模型

OSI参考模型

| 层数 | 名称       | 功能                                                         |
| ---- | :--------- | ------------------------------------------------------------ |
| 7    | 应用层     | 为应用程序提供服务并规定应用程序中通信相关的细节。包括文件传输、电子邮件、远程登录等协议。 |
| 6    | 表示层     | 将应用处理的信息转换为适合网络传输的格式，或将来自下一层的数据转换为上层能够处理的格式。因此它主要负责数据格式的转换。 |
| 5    | 会话层     | 负责建立和断开通信连接（数据流动的逻辑通路），以及数据的分割等数据传输相关的管理。 |
| 4    | 传输层     | 起着可靠传输的作用。只在通信双方节点上进行处理，而无需在路由器上处理。 |
| 3    | 网络层     | 将数据传输到目标地址。目标地址可以是多个网络通过路由器连接而成的某一个地址。`因此这一层主要负责寻址与路由选择` |
| 2    | 数据链路层 | 负责物理层面上的互连的、节点之间的通信传输。将0、1序列划分为具有意义的数据帧传送给对端（数据帧的生成与接收）。 |
| 1    | 物理层     | 负责0、1比特流（0、1序列）与电压的高低、光的闪灭之间的互换。 |

##### 总结：

* 第七层：应用层，定义要发送的数据内容
* 第六层：表示层，将数据从主机特有的格式转换为网络标准传输格式
* 第五层：会话层，确定才用哪个连接方式进行发送
* 第四层：传输层，确定连接与断开连接重发
* 第三层：网络层，从主机A到主机B的数据通信处理
* 第二层：数据链路层，和物理层一起向物理地址发送信号
* 第一层：物理层，