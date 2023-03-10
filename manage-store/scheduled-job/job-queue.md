# Job Queue

Mustom use RabbitMQ as a job queue. You can install RabbitMQ on your server, or you can use cloud based MQ services.

There are two kind of job queue. One is for ordinary task queue, and the other is for high latency task queue(HLTQ). Every queued tasks will be enqued to RabbitMQ, and then will dequeued and execueted one by one.

The difference between ordinary tasks and high latency tasks are resouce checking process. System will check CPU availablity and Memory availability before executing high latency tasks. If resources are not enough to execute high latency tasks, it will not executed, and will executed later when resouces are become available.

### Some of queued tasks

* Send Transaction Email
* Generate PDF Invoice
* Export Data (HLTQ)
* Generate Report Data (HLTQ)
* Generate Rule Based Coupon Code (HLTQ)

You can check the status and result of high latency task through a database table 'm\_core\_high\_latency\_task\_queue'.
