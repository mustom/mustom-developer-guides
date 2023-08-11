# Install Node.js & NPM

> This guide only cover NPM and Node.js installation on Ubuntu. There are several other way of Node.js & NPM installation, and you could install Node.js on other OS. You could find it easily by searching internet. (e.g. [https://docs.npmjs.com/downloading-and-installing-node-js-and-npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm))



STEP 1. Run the following command to download and execute the NodeSource installation script.

```
curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -

// You can specify node version by changing 'setup_16.x'. (e.g. setup_17.x)
```



STEP 2. Install Node.js

```
sudo apt install nodejs
```



STEP 3. Check Node.js version

```
node -v

// OUTPUT : v16.14.0 or Higher
```



STEP 4. Check NPM version

```
npm -v

// OUTPUT : 8.3.1 or Higher
```

