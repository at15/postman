# Choose a proper message queue

We need 

- persistent
- relatively high performance
- restart of mq itself won't cause trouble
- restart of client won't cause trouble
- have php client
- have nodejs client

We will

- create a job in the php client and push it to the queue
- * the node client will get the job and store it to monogodb
- some worker will finish the job
- tell the php client if it has provided hooks for this job
- allow php client to query status for a submitted job

- Apache kafka's php client is a extension, which is not good, and it doesn't support
new protocol, however, php client can use REST API provided by postman.

- Redis is fast and easy to use, but enable persistent will cause trouble for application
using redis as cache, this is a big problem for those who have to run everything on the same
machine.