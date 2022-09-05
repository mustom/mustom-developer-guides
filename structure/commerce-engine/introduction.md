# Introduction

> Commerce Engine is backbone of your store. Unlike ordinary ecommerce solution, it's totally decoupled from storefront, and even admin-panel. Commerce engine handle important business logic like transaction, and keep communicate with them using REST api. It also take care of data in database.

## Platform

Commerce engine built with Node.js and it's popular middleware Express. And they are used for web server.

The database that Mustom use is MariaDB, and it use Sequelize as a ORM. (The very first version of Mustom applied Mongo DB. But I decided that the relational database management system is the better choice for ecommerce system.)

Beside Node.js and Maria db, Mustom use several modules like node mailer(as a SMTP mail sender), winston(as a logger). I tried not to use bunch of module, and non popular modules, because they can cause maintenance issue.
