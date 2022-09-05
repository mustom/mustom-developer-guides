# Install MariaDB





1\. Update APT

```
sudo apt update
```

2\. Install MariaDB server using APT

```
sudo apt install mariadb-server
```

3\. Run security script

```
sudo mysql_secure_installation
```

4\. Security script will take you through a series of prompts. Below is kind of general example. You can choose another option.

```
...
NOTE: RUNNING ALL PARTS OF THIS SCRIPT IS RECOMMENDED FOR ALL MariaDB
      SERVERS IN PRODUCTION USE!  PLEASE READ EACH STEP CAREFULLY!

In order to log into MariaDB to secure it, we'll need the current
password for the root user. If you've just installed MariaDB, and
haven't set the root password yet, you should just press enter here.

Enter current password for root (enter for none):
OK, successfully used password, moving on...

// Press Enter

Setting the root password or using the unix_socket ensures that nobody
can log into the MariaDB root user without the proper authorisation.

You already have your root account protected, so you can safely answer 'n'.

Switch to unix_socket authentication [Y/n] n
 ... skipping.

// Enter n, not swich to unix_socket authentication

You already have your root account protected, so you can safely answer 'n'.

Change the root password? [Y/n] Y
New password:

// Enter New Password

Re-enter new password:

// Re-Enter new password.

Password updated successfully!
Reloading privilege tables..
 ... Success!


By default, a MariaDB installation has an anonymous user, allowing anyone
to log into MariaDB without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.

Remove anonymous users? [Y/n] Y
 ... Success!
 
 // Enter Y

Normally, root should only be allowed to connect from 'localhost'.  This
ensures that someone cannot guess at the root password from the network.

Disallow root login remotely? [Y/n] Y
 ... Success!
 
// Enter Y

By default, MariaDB comes with a database named 'test' that anyone can
access.  This is also intended only for testing, and should be removed
before moving into a production environment.

Remove test database and access to it? [Y/n] Y

// Enter Y

 - Dropping test database...
 ... Success!
 - Removing privileges on test database...
 ... Success!

Reloading the privilege tables will ensure that all changes made so far
will take effect immediately.

Reload privilege tables now? [Y/n] Y

// Enter Y

 ... Success!

Cleaning up...

All done!  If you've completed all of the above steps, your MariaDB
installation should now be secure.

Thanks for using MariaDB!OK, successfully used password, moving on...
```

5\. Access MariaDB

```
mysql -u root -p
```

6\. Create Database (You can change mustom to what ever)

```
MariaDB [(none)]> CREATE DATABASE mustom;
```
