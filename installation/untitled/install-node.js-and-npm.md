# Install Node.js & NPM

> This guide only cover NPM and Node.js installation on Ubuntu. There are several other way of Node.js & NPM installation, and you could install Node.js on other OS. You could find it easily by searching internet. (e.g. [https://docs.npmjs.com/downloading-and-installing-node-js-and-npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm))



STEP 1. Run the following command to download and execute the [NodeSource](https://github.com/nodesource/distributions#deb) installation script.

```
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash - &&\
sudo apt-get install -y nodejs
```



STEP 2. Install Node.js

```
sudo apt install nodejs
```



STEP 3. Check Node.js version

```
node -v

// OUTPUT : vXX.XX.X
```



STEP 4. Check NPM version

```
npm -v

// OUTPUT : X.X.X
```

