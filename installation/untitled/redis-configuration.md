# Redis Configuration

<mark style="color:red;">If you installed redis on your local environment on port 6379, you don't need to change configuration unless you need to set additional option.</mark>&#x20;



#### Steps to Change Redis Configuration

You can set host or port by changing config.json file.&#x20;

1. Navigate and open '/engine/system/redis/config/config.json'
2. Enter redis URL and save file

```json
{ 
    "url": "redis://alice:foobared@awesome.redis.server:6380"
}
```

GeneralURL format is 'redis\[s]://\[\[username]\[:password]@]\[host]\[:port]\[/db-number]'&#x20;

You can set addtional options like discrete parameters, UNIX sockets, and TLS. Please visit below link for more information.&#x20;

[https://github.com/redis/node-redis/blob/HEAD/docs/client-configuration.md](https://github.com/redis/node-redis/blob/HEAD/docs/client-configuration.md)

