# Go Lang

[Go](https://golang.org/)  
[Wiki](https://github.com/golang/go/wiki)

## Install

Make sure to uninstall old version first.

[Download](https://golang.org/dl/)

## Uninstall

```bash
sudo rm -rf /usr/local/bin/go
sudo rm -rf /etc/paths.d/go
```

## Modules Quick Start

The details are covered in the remainder of this page, but here is a simple example of creating a module from scratch.

Create a directory outside of your GOPATH:
```
$ mkdir -p /tmp/scratchpad/hello
$ cd /tmp/scratchpad/hello
```

Initialize a new module:
```
$ go mod init github.com/you/hello

go: creating new go.mod: module github.com/you/hello
```

Write your code:
```
$ cat <<EOF > hello.go
package main

import (
    "fmt"
    "rsc.io/quote"
)

func main() {
    fmt.Println(quote.Hello())
}
EOF
```

Build and run:
```
$ go build 
$ ./hello

Hello, world.
```

The `go.mod` file was updated to include explicit versions for your dependencies, where `v1.5.2` here is a [semver](https://semver.org) tag:
```
$ cat go.mod

module github.com/you/hello

require rsc.io/quote v1.5.2
```

Note there was no `go get` required. 

Your typical day-to-day workflow can be:

* Add import statements to your `.go` code as needed.
* Standard commands like `go build` or `go test` will automatically add new dependencies as needed to satisfy imports (updating `go.mod` and downloading the new dependencies).
* When needed, more specific versions of dependencies can be chosen with commands such as `go get foo@v1.2.3`, `go get foo@master`, `go get foo@e3702bed2`, or by editing `go.mod` directly.  

### Best Practices
https://blog.learngoprogramming.com/code-organization-tips-with-packages-d30de0d11f46  
https://blog.learngoprogramming.com/special-packages-and-directories-in-go-1d6295690a6b  
https://rakyll.org/style-packages/  
https://medium.com/@benbjohnson/standard-package-layout-7cdbc8391fc1#.ds38va3pp  
https://peter.bourgon.org/go-best-practices-2016/#repository-structure  
https://www.ardanlabs.com/blog/2017/02/design-philosophy-on-packaging.html  
https://www.youtube.com/watch?v=spKM5CyBwJA  

### Linters
https://github.com/golangci/golangci-lint

### Learn More
https://github.com/magefile/mage

### Issues
https://medium.com/@leeprovoost/suppressing-accept-incoming-network-connections-warnings-on-osx-7665b33927ca

### Useful commands

```bash 
go run hello.go
go install hello.go
```


