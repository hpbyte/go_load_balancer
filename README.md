# Simplest Load Balancer written with Go

It uses the Round Robin algorithm to load-balance the backends and have a retry mechanism.

### How to run

Create a few simple HTTP backends and run:
```
go run main.go -backends="http://localhost:8081,http://localhost:8082,http://localhost:8083,http://localhost:8084"
```

Test the load balancer

```
curl http://localhost:3030
```
