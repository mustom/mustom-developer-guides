# Job Queue

Mustom use RabbitMQ as a job queue.

There are two kind of job queue. One is for ordinary tasks, and the other is for high latency tasks. Every queued tasks will be enqued to RabbitMQ, and then will dequeued and execueted one by one. The difference between ordinary tasks and high latency tasks are resouce checking process. System will check CPU availablity and Memory availability before executing high latency tasks. If resources are not enough to execute high latency tasks, it will not executed, and will executed later when resouces are become available.

