# SSL

> You MUST use SSL for your store. It is mandatory for your business. But, if you don't want to use SSL for some reason(e.g. test environment), you need to un-comment some lines.&#x20;

## Case 1. Use SSL

1\. Copy/paste SSL certificate files to '/configuration/ssl'

2\. Change key, cert, ca file name in index.js

```
...
const https = require('https')
const options = {
    key: fs.readFileSync(__dirname + '/config/ssl/YOUR-SSL-KEY-FILE'),
    cert: fs.readFileSync(__dirname + '/config/ssl/YOUR-SSL-CERT-FILE'),
    ca: fs.readFileSync(__dirname + '/config/ssl/YOUR-SSL-CA-FILE')
}
https.createServer(options, app).listen(443)
...
```

If your cert format is different (e.g. pfx), above code should be changed like this.

```
...
const https = require('https')
const options = {
    pfx: fs.readFileSync(__dirname + '/config/ssl/YOUR-PFX-FILE'),
    passphrase: 'example'
}
https.createServer(options, app).listen(443)
...
```

## Case 2. Not Use SSL

In case you don't want to use SSL, comment below lines in index.js. (You only need line 2\~3, if you don't use SSL)

```
// Node Server Start - HTTP
const http = require('http')
http.createServer(app).listen(80)


// Node Server Start - HTTPS
// Comment below codes, if you don't use SSL
// const https = require('https')
// const options = {
//     key: fs.readFileSync(__dirname + '/config/ssl/berrysix.com_key.txt'),
//     cert: fs.readFileSync(__dirname + '/config/ssl/berrysix_com.crt'),
//     ca: fs.readFileSync(__dirname + '/config/ssl/berrysix_com.ca-bundle')
// }
// https.createServer(options, app).listen(443)


// Redirect HTTP to HTTPS
// Comment below codes, if you don't use SSL
// app.all('*', (req, res, next) => {
//     if (req.secure) { 
//         next()
//     } else { 
//         res.redirect('https://' + req.hostname + req.url)
//     } 
// })
```
