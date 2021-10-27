`go run` will compile and run the program but it doesn't create a executable file.
`go build` Will compile and create a executable file.

A package is a collection of source files grouped in a single directory.

```
package main
import "fmt"

func main() {
    fmt.Println("Hello, world!")
}
```

You can call functions defined in the same package without needing to import the
package.

Packages
with the name main will contain a function named main(), which serves as an
entry point for your program to get started.

Cross compiling using go
`$ GOOS=windows GOARCH=amd64 go build -o output.exe`

We could specify output file with -o option.

Install go tools to solve problems in vs code using:
ctrl + shift + p then Go Install/Update -> Select all package and press Enter to install.

To build a package and prevent from getting function undecleard in same package
use this methods
create module with 
`$ go mod init <module_name>`
or change value of the go env variable GO111MODULE to auto
`$ export GO111MODULE=auto`


