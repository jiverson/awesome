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

### Best Practices
https://blog.learngoprogramming.com/code-organization-tips-with-packages-d30de0d11f46  
https://blog.learngoprogramming.com/special-packages-and-directories-in-go-1d6295690a6b  
https://rakyll.org/style-packages/  
https://medium.com/@benbjohnson/standard-package-layout-7cdbc8391fc1#.ds38va3pp  
https://peter.bourgon.org/go-best-practices-2016/#repository-structure  
https://www.ardanlabs.com/blog/2017/02/design-philosophy-on-packaging.html  
https://www.youtube.com/watch?v=spKM5CyBwJA  


### Learn More
https://github.com/magefile/mage


### Useful commands

```bash 
go run hello.go
go install hello.go
```


