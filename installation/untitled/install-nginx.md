# Install Nginx



> Node.js can run without Nginx. However, Mustom designed to run along with Nginx as a reverse proxy. (It is not recommended to run Mustom without NginX)



## Installation (Ubuntu)



Step 1. Update APT

```
sudo apt update
```



Step 2. Install Nginx using following command

```
sudo apt install nginx
```



Step 3. After the installation is complete, you can check it was installed successfully and see the installed version.

```
nginx -v

// Output
nginx version: nginx/1.18.0 (Ubuntu)
```



STEP 4. At the end of the installation process, Ubuntu starts Nginx. You can confirm that the nginx service is up and running through the command below.

(By default, Nginx is configured to start automatically when the server boots)

```
sudo systemctl status nginx
```



Step 5. If you're running a system firewall,  allow access to Nginx.

```
sudo ufw allow 'NGINX Full'
```



Step 6. Open your browser, and enter your server's IP address. Everything is OK, you will see the page below.

<figure><img src="../../.gitbook/assets/nginx.JPG" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If you cannot install Nginx successfully using the method described above, try the alternative procedures listed on the [Nginx installation guide](https://www.nginx.com/resources/wiki/start/topics/tutorials/install/) .
{% endhint %}



## Configure TLS (SSL)

You need to have TLS



## General Configuration

Step 1. We will create a server block configuration file. Move to '/etc/nginx/sites-available/' folder

```
cd /etc/nginx/sites-available/
```



Step 2. Generate a file with your actual domain name. (e.g. mustom.com)

```
nano your_domain
```



Step 3. Enter .. and save file

```
server {
    server_name <your_domain>;

    location / {
        proxy_pass <http://localhost:3000>;
    }
}
```



Step 4. Back to your terminal and create a symbolic link of this your\_domain file in the '/etc/nginx/sites-enabled' folder

```
sudo ln -s /etc/nginx/sites-available/your_domain /etc/nginx/sites-enabled/your_domain
```



Step 5. Reload NginX configuration

```
sudo nginx -s reload
```



## Advanced Configuraion
