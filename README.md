﻿# .net core dotnetty tcp server (jt808)

在网上看到Azure团队开源的DotNetty框架，一时兴起写了个基于DotNetty的Tcp Server Demo
解析了JT808的部分指令，应答部分暂时未弄完，代码写的比较随意请不要在意。

部分代码参考了java版本的jt808协议解析 https://github.com/hylexus/jt-808-protocol

感慨JAVA强大的同时，还是喜欢C#强大的语法，希望.net core发展越来越好

直接运行程序，端口默认9623（在Main方法里面修改），可以使用网络调试助手联调（Tool\NetAssist.exe）

![Image text](https://github.com/mingyunet/JT808-Server/blob/master/Tool/data.png)


# 部分JT808测试数据如下：

## 终端注册
7E0100002c0200000000150025002c0133373039363054372d54383038000000000000000000000000003033323931373001d4c142383838387b7E

## 终端鉴权
7E0102000B018170223038009D3138313730323233303338787E 

## 轨迹数据
7E0200007D020181702230330003000000000000000101EA3B5906AFC37000000000000018050921435330011F310100D004000A0000D40164E10201A4E221545A43532D312E31332E3130392E342031372D31322D32382C4D5430335F503130E30F343630303031383633353537393237E41301CC0000708177443E7081C1A43D7081774535E504012C02580E7E

## 终端心跳
7E0002000001817022303801B8617E
