NATS Server is written in Go and available across multiple platforms. The server uses a text based protocol making it accessible to clients created in different languages.

#### Task

The first step to launching NATS is to download the pre-built binary from Github.

The command below will download and unzip the binary onto the first host.

`curl -OL https://github.com/nats-io/gnatsd/releases/download/v0.9.6/gnatsd-v0.9.6-linux-amd64.zip && unzip gnatsd-v0.9.6-linux-amd64.zip`{{execute HOST1}}
