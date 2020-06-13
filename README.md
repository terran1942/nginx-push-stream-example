# Nginx publisher
## 环境要求
+ Ubuntu server 18.04

## 编译安装
``` bash
apt update
apt upgrade -y
apt install libpcre3-dev libssl-dev openssl zlib1g-dev
apt autoremove
wget https://nginx.org/download/nginx-1.18.0.tar.gz
git clone https://github.com/wandenberg/nginx-push-stream-module.git
tar -xzcf nginx-1.18.0.tar.gz
cd nginx-1.18.0
./configure --add-module=../nginx-push-stream-module
```
