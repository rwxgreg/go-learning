# Chapter 1. Install and setup environment

## Windows

💾 Install [go1.23.2.windows-amd64.msi](https://go.dev/dl/)

or

`choco install golang`

## Go mod init
`go mod init hello_world `

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

## Go build
`go build`

## Veryfication
`go fmt ./...` - automatically correct code syntax
`go vet ./...` - check whose arguments do not align with the format

## Make installation and run
`choco install make`

```
.DEFAULT_GOAL := build
.PHONY:fmt vet build
fmt:
	go fmt ./...
vet: fmt
	go vet ./...
build: vet
	go build
```

`make`

