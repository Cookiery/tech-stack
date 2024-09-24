# Install

## 1. Official Install

https://go.dev/dl/

```bash
wget https://go.dev/dl/go1.21.0.linux-amd64.tar.gz // wget 用不了可以从本地 scp 直接上传
// scp 的话可以这样用：scp go1.21.0.linux-amd64.tar.gz root@118.25.143.182:/root/env
tar -xzf go1.20.7.linux-amd64.tar.gz
export PATH=$PATH:/root/env/go/bin/
go version

mkdir /root/env/gopath // 在 env 里创建一个 gopath 的目录
rm -rf /root/go // 把主目录下的 go 删了
vim ~/.bashrc 
// 把下面两行加进去
export PATH=$PATH:/root/env/go/bin/
export GOPATH=/root/env/gopath

source ~/.bashrc

// 这个时候用 go env 命令就可以看到
GOMODCACHE='/root/env/gopath/pkg/mod'
GOPATH='/root/env/gopath'
```