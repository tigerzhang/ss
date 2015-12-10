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

## Windows
进入 win_ss 文件夹
编辑 config.txt文件, 把`<ip>`和`<password>`换成相应的ip和密码
```json
{

    "server":"<ip>",
     "server_port":8388,
    "local_port":1080,
    "password":"<password>",
    "method": "aes-128-cfb",
    "timeout":600
}
```
双击 ss_win.bat
在浏览器设置 SOCKS v5 代理

# ssh over socks proxy
```bash
alias sshs="ssh -o ProxyCommand='nc -x 127.0.0.1:1080 %h %p'"
sshs <username>@<hostname> [-p <port>]
```
