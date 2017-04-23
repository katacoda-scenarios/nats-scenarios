With the NATS Server deployed we can start the service and connect to it from a client. As mentioned in the previous step, because the server is a text based protocol, a simple client such as _telnet_ is enough.

#### Start Server

The command below will start the server using the first host in the background via _nohup_. By default, NATS listens on port _4222_.

`nohup ./gnatsd-v0.9.6-linux-amd64/gnatsd  </dev/null &>/dev/null &`{{execute HOST1}}

#### Start Client Host 1

To begin, connect to the running server from our first host.

`telnet [[CLIENT_IP]] 4222`{{execute HOST1}}

After connecting, the client receives a JSON block detailing information about the server.

#### Start Client Host 2

We'll then connect our second client to the same server.

`telnet [[CLIENT_IP]] 4222`{{execute HOST2}}
