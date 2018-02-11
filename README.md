# name_server
> 用于测试linux fd跨进程转移的例子

## 编译
`make`

## 使用
1. `./server 127.0.0.1 1234 10`
 启动server，绑定地址127.0.0.1:1234,启动10个子进程

2. `./client 127.0.0.1 1235 1234`
  启动client，绑定地址127.0.0.1:1235,并连接127.0.0.1:1234
  输入`0  123123`，即向server的0号进程发送消息。支持多次输入，支持切换进程编号。
