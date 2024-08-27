# gRPC-GO

An example of how to use gRPC with HTTP/2 to send and receive messages with Golang.

##Install gRPC
<pre>
$ apt install -y protobuf-compiler
$ protoc --version  # Ensure compiler version is 3+
</pre>

##Install GO gRPC libraries
<pre>
$ go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
$ go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
</pre>

##Run gRPC proto
**--go_out** Generates the entity of the messages informed in the proto file
**--go-grpc_out** Generates files and interfaces to make communication.
<pre>
protoc --go_out=. --go-grpc_out=. proto/course_category.proto
</pre>
The **pb** directory should be created.
