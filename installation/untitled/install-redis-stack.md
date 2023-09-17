# Install Redis Stack



> To enhance performance, Mustom uses Redis as a in-memory cache. For instance, the product data used for product listing pages comes from Redis, not the database. To install Mustom, you need to install 'Redisearch' and 'RedisJSON', as well as Redis. So, we will install 'Redis Stack'





## Install Redis Stack

{% hint style="info" %}
Please visit [official website](https://redis.io/docs/getting-started/install-stack/linux/) for detailed installation guide.
{% endhint %}



STEP 1. Add official `packages.redis.io` APT repository to the APT index. Firstly, you need to download key through the command below.

```
curl -fsSL https://packages.redis.io/gpg | sudo gpg --dearmor -o /usr/share/keyrings/redis-archive-keyring.gpg
```



STEP 2. Modify file permission

```
sudo chmod 644 /usr/share/keyrings/redis-archive-keyring.gpg
```



STEP 3. Creating a new `.list` File in `sources.list.d`

```
echo "deb [signed-by=/usr/share/keyrings/redis-archive-keyring.gpg] https://packages.redis.io/deb $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/redis.list
```



STEP 4. Update APT

```
sudo apt-get update
```



STEP 5. Install Redis Stack Server

```
sudo apt-get install redis-stack-server
```
