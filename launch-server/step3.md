NATS Server has Sub/Pub features. By subscribing, you will receive all the messages other clients send to it.

#### Subscribe
On the first host, we'll subscribe to all messages of _foo_ and we'll assign an ID of 1.
`SUB foo 1`{{execute HOST1}}

#### Publish

One the second client we'll publish a message _Hello World_ to _foo_ with an ID of 11.

`PUB foo 11
Hello World`{{execute HOST2}}

On the first host, you'll see the message sent.
