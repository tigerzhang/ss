# Usage

## Mac64
```bash
$ chmod a+x ss
$ ./ss <host> <password>
```

## Linux
```bash
$ chmod a+x ss_linux
$ ./ss_linux <host> <password>
```


# ssh over socks proxy
```bash
alias sshs="ssh -o ProxyCommand='nc -x 127.0.0.1:1080 %h %p'"
sshs <username>@<hostname> [-p <port>]
```

# 问题
目前只支持 Mac64, Linux 客户端，Windows 后续增加。
