# grpc-diner

A gRPC example. Copy from [protoc-grpcio](https://github.com/mtp401/protoc-grpcio).

## Requirements

- You must have Google's Protocol Buffer compiler (`protoc`) installed and in
  `PATH`.

You can install protobuf (include `protoc`) in macOS using below command:
```Bash
brew install protobuf
```

## Run

You can inspect this example by compiling and running the example server in one shell session:
```Bash
cargo run --bin server
    Finished dev [unoptimized + debuginfo] target(s) in 0.18s
     Running `target/debug/server`
listening on 127.0.0.1:59519
```

And then running the client in another:
```Bash
cargo run --bin client 59519
    Finished dev [unoptimized + debuginfo] target(s) in 0.13s
     Running `target/debug/client 59519`
Ate: items: SPAM items: EGGS and got charged $0.30
```

