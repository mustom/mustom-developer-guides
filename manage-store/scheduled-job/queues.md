# Queues

## Task Queue

Mustom use RabbitMQ as a task (work/job) queue. You can install RabbitMQ on your server, or you can use cloud based MQ services. Written below is some tasks that use RabbitMQ.

* Send Transaction Email
* Generate PDF Invoice
* Export Data
* Generate Report Data
* Generate Rule Based Coupon Code

There are three kind of task queues.&#x20;

#### Express Queue

This queue will handle ordinary tasks like leaving a admin action logs. Mustom use topic based exchange for this queue. (You can save task result in database by passing a arguement)

#### Email Queue

It will handle email delivery. Mustom use worker queue for this queue.

#### Heavy Load Queue

This queue is a little bit unique. The difference between ordinary tasks and high latency tasks are resouce checking process. System will check CPU availablity and Memory availability before executing high latency tasks. If resources are not enough to execute high latency tasks, it will not executed, and will executed later when resouces are become available. You can check the status and result of high latency task through a database table 'm\_core\_high\_latency\_task\_queue'.



## Queue for System Health Check

It is very different from task queue. When publisher (schedule) publish event, all of workers(subscribers) are listen this event, and then report system status. So that we can check status of each instances, and clusters. (If certain environment is out of service, additional action will be take place. For instance, other environment will be handle scheduled task (cron), if this environment handle this.)&#x20;
