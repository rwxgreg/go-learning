# Chapter 1. Install and setup environment

## Windows

💾 Install [go1.23.2.windows-amd64.msi](https://go.dev/dl/)

## Create your GOPATH

The `GOPATH` is where all your Go code will live.

Create new folder `C:\GoPath`

Go to the `System` --> `Advanced` --> `Environment Variables` --> `System variables`:

 * Add `GOPATH` with value `C:\GoPath`

Veryfication:   
`PS C:\REPO\github\go-learning> go version`    
`go version go1.23.2 windows/amd64`

## Hello, world!

```
package main

import "fmt"

func main() {
    fmt.Println("Hello, world!")
}
```
```
PS C:\REPO\github\go-learning> go run code\hello_world.go
Hello, world!
```

Info:   
`package` -  is a one or more go source files, something like box for it    
`import` -  bringing the specified package from its source location to the destination code, wiz the main program   
