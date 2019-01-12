# Go Lang

[Go](https://golang.org/)

## Install

Make sure to uninstall old version first.

[Download](https://golang.org/dl/)

```bash
vim ~/.zshrc

# add the following
export GOPATH=$HOME/go-workspace
export GOBIN=$GOPATH/bin
export PATH=$GOPATH/bin:$PATH

source ~/.zshrc
```

## Uninstall

```bash
sudo rm -rf /usr/local/bin/go
sudo rm -rf /etc/paths.d/go
```
