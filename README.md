# XRAY CRACKER

### 生成证书

使用 `-g username` 生成永久证书

```shell
# ./xray-cracker -g kali

证书已写入文件：xray-license.lic
```

### 破解 xray

目前支持版本：

- amd64 Windows
- amd64 Linux
- amd64 MacOS

使用 `-c path-to-xray` 自动patch二进制xray

```bash
# ./xray-crack.exe -c xray_linux_amd64
linux amd64
[.text] offset: 0x1000, addr: 0x401000-0x11787e3
Signature last index: 0xae2f2e
Patch success: xray_linux_amd64
```

## 破解效果

使用修改版 xray 和永久证书后，效果如下

```shell
# xray_windows_amd64.exe version

____  ___.________.    ____.   _____.___.
\   \/  /\_   __   \  /  _  \  \__  |   |
 \     /  |    _  _/ /  /_\  \  /   |   |
 /     \  |    |   \/    |    \ \____   |
\___/\  \ |____|   /\____|_   / / _____/
      \_/       \_/        \_/  \/

Version: 1.4.0/5ce0e903/COMMUNITY-ADVANCED
Licensed to abc, license is valid until 2099-09-09 08:00:00

[xray 1.4.0/5ce0e903]
Build: [2020-11-06] [windows/amd64] [RELEASE/COMMUNITY-ADVANCED]
Compiler Version: go version go1.14.4 linux/amd64
License ID: 00000000000000000000000000000000
User Name: abc/00000000000000000000000000000000
Not Valid Before: 2020-06-12 00:00:00
Not Valid After: 2099-09-09 08:00:00

To show open source licenses, please use `osslicense` sub-command.
```
