# Tutorial 1

---

To indicates an executable program. The Go runtime looks for the main function within this package to start execution.

That is why the "main" keyword is used as seen below:

```go
package main
```

Else, Go runtime will see it as a library package which can be imported or used by other Go developers.

```go
package mylib
```

---


### How to comment in GO:

1. Single-line comments: These start with // and extend to the end of the line.

    ```go
    // This is a single-line comment
    ```
2. Multi-line comments: These start with /* and end with */. They can span multiple lines.

    ```go
    /*
    This is a multi-line comment.
    It can span multiple lines.
    */
    ```

---

### How to write a function in GO

```go
func functionName(parameters) returnType {
    // function body
}
```

---

### How to import a package in GO

```go
import "package/path"
```

---

### Difference between the "go run" and "go build" commands

#### *go run* command:

- Purpose: Quickly compile and run Go programs.
- Usage: go run filename.go
- Behavior: Compiles the specified Go source file(s) and immediately runs the resulting executable. It does not produce a standalone executable file on disk.
- Use Case: Ideal for quick testing and running small scripts or programs during development.

```go
go run main.go
```

#### *go build* command:

- Purpose: Compile Go programs and produce a standalone executable file.
- Usage: go build [package]
- Behavior: Compiles the specified package (or the package in the current directory if none is specified) and produces an executable file in the current directory. The executable can be run independently of the Go toolchain.
- Use Case: Useful for creating production-ready binaries that can be distributed and run on other systems.

```go
go build main.go
```

