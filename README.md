# go-websocket-chat
网上找的go websocket学习例子，自己重新整理，加注释调试，便于理解代码执行流程。

先注册用户基本信息，用户名，socket连接，消息体等，同时把所有用户存储好，循环开始发送消息。

第一次请求 ws://127.0.0.1:8090/ws 建立连接
第二次请求 发送 {"type":"login","content":"x1"} 登录
第三次请求 发送 {"type":"user","content":"消息"}发送消息

在线用户列表存在每一个单独在线用户而不是全局
