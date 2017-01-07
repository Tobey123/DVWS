# Damn Vulnerable Web Sockets (DVWS)
Damn Vulnerable Web Sockets (DVWS) is a vulnerable web application which works on web sockets for client-server communication. The flow of the application is similar to [DVWA](https://github.com/ethicalhack3r/DVWA). You will find more vulnerabilities than the ones listed in the application.

## Requirements
In the ```hosts``` file of your attacker machine create an entry for ```dvws.local``` to point at the IP address hosting the DVWS application.

Location of ```hosts``` file:

Windows: ```C:\windows\System32\drivers\etc\hosts```

Linux: ```/etc/hosts```

Sample file:
```
dvws.local         192.168.100.199
```

The application requires the following:

Apache + PHP + MySQL

PHP with MySQLi support

[Ratchet](https://github.com/ratchetphp/Ratchet)

[ReactPHP-MySQL](https://github.com/bixuehujin/reactphp-mysql/)

## Setting up DVWS
Set the MySQL hostname, username, password and an existing database name in the ```includes/connect-db.php``` file then go to Setup to finish setting up DVWS.

## Running DVWS
On the host running this application, run the following command from DVWS directory: ```php ws-socket.php```

## Important Note
DVWS has been developed with limited knowledge of Web Sockets. Feel free to contribute and enhance this project.

## Screenshot
![image](https://cloud.githubusercontent.com/assets/5358495/21744585/a23a1968-d53e-11e6-9ce4-4dc85aa194b1.png)

