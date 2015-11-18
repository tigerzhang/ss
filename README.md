# Usage

```bash
$ chmod a+x ss
$ ./ss <host> <password>
```

# ssh over socks proxy
```bash
alias sshs="ssh -o ProxyCommand='nc -x 127.0.0.1:1080 %h %p'"
sshs <username>@<hostname> [-p <port>]
```

# 问题
目前只支持 Mac64 客户端，Linux/Windows 后续增加。
