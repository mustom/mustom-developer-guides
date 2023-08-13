# Install Redis



> To enhance performance, Mustom uses Redis as a inmemory cache. For instance, the product data used for product listing pages comes from Redis, not the database. To install Mustom, you need to install Redisearch module, RedisJSON module, as well as Redis.



## Install Redis on your Ubuntu server



Step 1 . Update APT

```
sudo apt update
```



Step 2. Install Redis

```
sudo apt install redis-server
```



Step 3. Check Redis version

```
redis-cli --version

// OUTPUT : 
// redis-cli 6.0.16
```



Step 4. Check status

```
sudo systemctl status redis
```



## Install Redis Stack

{% hint style="info" %}
You need to install Redis stack, because Mustom use it's feature 'RedisJSON' and 'Redisearch'. Please visit [official website](https://redis.io/docs/getting-started/install-stack/linux/) for detailed installation guide.
{% endhint %}

Add official packages.redis.io APT repository to the apt index, update it, and install it

```
curl -fsSL https://packages.redis.io/gpg | sudo gpg --dearmor -o /usr/share/keyrings/redis-archive-keyring.gpg

sudo chmod 644 /usr/share/keyrings/redis-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/redis-archive-keyring.gpg] https://packages.redis.io/deb $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/redis.list

sudo apt-get update

sudo apt-get install redis-stack-server
```

