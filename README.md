# HTTP Benchmark - Server

This program is a simple web server in go used as a benchmarking tool.

This webserver hosts a 1kb binary file *1kb.bin* generated with the command :

```bash
dd if=/dev/zero of=1kb.bin bs=1KB count=1
```

This server uses the port **8000** and the library gorilla/mux (https://github.com/gorilla/mux).

You can launch the server with the command :

```golang
go run .
```

or 

```golang
go build .
./httpbenchmark-server
```