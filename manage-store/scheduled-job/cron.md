# Cron



> Cron feature in Mustom is not a real cron tab that powered by operating system. Mustom just use node-cron library to manage scheduled tasks. But, we will still use the term 'cron' for easy understanding.

## How cron works in multiple instance/cluster envirionment

* Basically all process run a scheduled task named 'health-cheker'. This task will report system status and availablity.
* The other tasks are only run on #0 cluster, to avoid duplicated task execution.
* If there are multiple instances(servers), only #0 cluster of main host will handle scheduled tasks. In case main host is out of service, other host will hand over these schedule.

{% hint style="info" %}
Please report there are any issues related to this logic. The logic above is not verified, because I do not test it fully.
{% endhint %}



## Change Cron Schedule
