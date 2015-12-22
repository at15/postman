# postman
A unify wrapper for using third party API to send email, sms and push

![postman-logo](postman.png)

## Feature

* not implemented 

- * switch between multiple third party API, like switch to mailgun from qq.
- * webhook for client, notify them using specified callback when job finished
- * admin-ui to monitor usage and third party api status

## Road map

see [working](doc/working) for detail

- [ ] chose a message queue
- [ ] assign jobs to workers
- [ ] allow client to query job status and get results
- [ ] webhook for client, post them when some job have finished
- [ ] worker for send sms and email
- [ ] worker for send push messages
