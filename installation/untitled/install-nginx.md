# Install Nginx



> Node.js can run without Nginx. However, Mustom designed to run along with Nginx as a reverse proxy. (It is not recommended to run Mustom without NginX)



## Installation (Ubuntu)



STEP 1. Update APT

```
sudo apt update
```



STEP 2. Install Nginx using following command

```
sudo apt install nginx
```



STEP 3. After the installation is complete, you can check it was installed successfully and see the installed version.

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



STEP 5. Open your browser, and enter your server's IP address. Everything is OK, you will see the page below.

<figure><img src="../../.gitbook/assets/nginx.JPG" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
If you cannot install Nginx successfully using the method described above, try the alternative procedures listed on the [Nginx installation guide](https://www.nginx.com/resources/wiki/start/topics/tutorials/install/) .
{% endhint %}





## General Configuration





## Configure TLS (SSL)

You need to have TLS





## Advanced Configuraion
