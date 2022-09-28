# LySniffer 数据包抓包工具

<br>

<div align=center>
 
![image](https://user-images.githubusercontent.com/52789403/192729389-0ab902f4-fe2c-42b9-a93a-9022099efd62.png)
 
</div>

<br>

一款运用Npcap库开发的流量数据包解析工具，支持匹配过滤条件表达式，只是演示案例目前并不具备应用实战价值，放到此处作为案例。

 - 输出网卡信息
```C
Shell> LySniffer.exe --ShowAdapters
----------------------------------------------------------------------------------------------------
索引     网卡名
----------------------------------------------------------------------------------------------------
[ 1 ]    [ Network adapter 'WAN Miniport (Network Monitor)' on local host ]
[ 2 ]    [ Network adapter 'WAN Miniport (IPv6)' on local host ]
[ 3 ]    [ Network adapter 'WAN Miniport (IP)' on local host ]
[ 4 ]    [ Network adapter 'Microsoft Hosted Network Virtual Adapter' on local host ]
[ 5 ]    [ Network adapter 'VMware Virtual Ethernet Adapter for VMnet8' on local host ]
[ 6 ]    [ Network adapter 'VMware Virtual Ethernet Adapter for VMnet1' on local host ]
[ 7 ]    [ Network adapter 'Intel(R) Ethernet Connection (7) I219-LM' on local host ]

 网卡数量: 9
 ```
 
  - 获取TCP数据包
```C
Shell> LySniffer.exe --Monitor 7 --Type tcp

源端口:      0 --> 目标端口:      0 --> 窗口大小:       0 --> 标志: (0)None 未知
源端口:      0 --> 目标端口:      0 --> 窗口大小:       0 --> 标志: (0)None 未知
源端口:   1138 --> 目标端口:  36688 --> 窗口大小:      -1 --> 标志: (2)SYN 建立连接
源端口:  36688 --> 目标端口:   1138 --> 窗口大小:      -1 --> 标志: (18)ACK 响应
源端口:   1138 --> 目标端口:  36688 --> 窗口大小:     128 --> 标志: (16)ACK 响应
源端口:   1138 --> 目标端口:  36688 --> 窗口大小:     128 --> 标志: (24)PSH 数据传输
```
 






