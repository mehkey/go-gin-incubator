
# Go Gin Incubator

[Gin QuickStart Info](https://gin-gonic.com/docs/quickstart/)

> go mod init
> go mod tidy
> go run main.go 


[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"

```
❯ go run .
[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
 - using env:   export GIN_MODE=release
 - using code:  gin.SetMode(gin.ReleaseMode)

[GIN-debug] GET    /ping                     --> main.setupRouter.func1 (3 handlers)
[GIN-debug] GET    /user/:name               --> main.setupRouter.func2 (3 handlers)
[GIN-debug] POST   /admin                    --> main.setupRouter.func3 (4 handlers)
[GIN-debug] [WARNING] You trusted all proxies, this is NOT safe. We recommend you to set a value.
Please check https://pkg.go.dev/github.com/gin-gonic/gin#readme-don-t-trust-all-proxies for details.
[GIN-debug] Listening and serving HTTP on :8080
[GIN] 2022/12/26 - 21:48:12 | 404 |         470ns |             ::1 | GET      "/"
[GIN] 2022/12/26 - 21:48:25 | 200 |      14.491µs |             ::1 | GET      "/ping"
[GIN] 2022/12/26 - 21:49:16 | 200 |    1.277627ms |             ::1 | GET      "/user/foo"
[GIN] 2022/12/26 - 21:49:21 | 200 |      19.816µs |             ::1 | GET      "/user/abd"
[GIN] 2022/12/26 - 21:49:37 | 404 |         506ns |             ::1 | GET      "/admin"
```