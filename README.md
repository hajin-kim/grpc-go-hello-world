# gRPC with Go - Hello World

## Run on local environment

Install Go.

- Debian: `sudo apt install go`
- Red Hat: `sudo yum install go`
- MacOS: `brew install go`

Register the below PATH ENVIRONMENT VARIABLE.

`export PATH="$PATH:$(go env GOPATH)/bin"`

Setup the hello-world project.

```sh
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28
wget https://github.com/grpc/grpc-go/archive/v1.56.1.zip
unzip v1.56.1.zip
cd grpc-go-1.56.1/examples/helloworld/
```

Run the server.

`go run greeter_server/main.go &`

And then run the client.

`go run greeter_client/main.go`
