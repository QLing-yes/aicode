---
tags:
  - mklink
  - netsh
---
## 端口映射

[netsh微软文档](https://docs.microsoft.com/zh-cn/windows-server/networking/technologies/netsh/netsh-interface-portproxy)
[微信文章](https://mp.weixin.qq.com/s/ULbumPtqPzRxymX16htm3A)

```
选项: <add,del,show,reset,set,> <v4tov4,v4tov6, v6tov4, v6tov6> 

示例: netsh.exe interface portproxy add v6tov4 listenport=6000 listenaddress=* connectport=6000 connectaddress=127.0.0.1
```

## 符号链接

```
mklink [[/d] | [/h] | [/j]] <link> <target>
```

| Parameter  | Description                    |
| ---------- | ------------------------------ |
| /d         | 创建目录符号链接。默认情况下，此命令会创建一个文件符号链接。 |
| /h         | 创建硬链接而非符号链接。                   |
| /j         | 创建目录连接。                        |
| `<link>`   | 指定要创建的符号链接的名称。                 |
| `<target>` | 指定新符号链接所指的路径 (相对或绝对)。          |
| /?         | 在命令提示符处显示帮助。                   |