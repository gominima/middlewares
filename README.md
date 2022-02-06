# Middlewares

This is a base stack for minima, for more middlewares you could check [Goware](https://github.com/goware) or [Go-Chi](https://github.com/Go-Chi)

## Credit

All the middlewares here are ported over from [Go-Chi's middlewares](https://github.com/go-chi/chi/tree/master/middleware)


## ⚙️ Setup

```bash
go get github.com/gominima/minima

go get github.com/gominima/middlewares
```

## 📑 Example

```go
package main

import ("github.com/gominima/minima"
        "github.com/gominima/middleware")

func main() {
	app := minima.New()
        app.UseRaw(middleware.Logger())
	app.Listen(":3000")
}

```
