# SSL/TLS

> You MUST use SSL/TLS for your store. It is mandatory for your business.

1\. Copy/paste SSL/TLS certificate files to some place like '/engine/config/tls'.

2\. Navigate to '/engine/config/ and open 'TLS.json' file.

3\. Change TLS.json file like this.

_<mark style="color:red;">Please note that the key name 'key', 'cert', 'ca' should not be changed. And the value is the path that your cert file is located.</mark>_

```
{ 
    "key": "/config/tls/yourstore.com_key.txt",
    "cert": "/config/tls/yourstore_com.crt",
    "ca": "/config/tls/yourstore_com.ca-bundle"
}
```

If your cert format is different (e.g. pfx), above code should be changed like this.

```
{
    "pfx": "/config/ssl/YOUR-PFX-FILE",
    "passphrase": "example"
}
```



## Case 2. Not Using SSL/TLS

In case you don't want to use SSL, you need to change .env file.

_<mark style="color:red;">Actually, Installer have this configuration. So, you don't need to set it again, if you set this correctly while installation process.</mark>_

1. Move to engine root folder, and open .env file.
2. Change the value of USE\_TLS to false.

```
...
# ----------------------------------------------------------
# USE TLS OR HTTP (true / false)
# ----------------------------------------------------------
USE_TLS=false
...
```

