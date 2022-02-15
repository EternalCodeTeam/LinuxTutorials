# MariaDB (Mysql) Installation


## TODO: More Mysql menagment commands!

If you want to get help regarding our products or just want to ask something, join our [discord](https://discord.gg/MUCKhgFUCA).

#### Linux Update
```
sudo apt update && sudo apt upgrade -y
```

#### Add the additionals packets
```
sudo apt-get install software-properties-common
```

#### Install mariadb-server

```linux
sudo apt install mariadb-server
``` 

#### Check the mariadb status
```linux
sudo systemctl status mariadb
```

#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154024692-03df9fe3-113e-4047-a71b-f9e89c8dbf78.png)

#### Check the mysql version

```linux 
mysql -v
```
#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154025047-df08e9ab-4016-4bf6-8e6e-5e16fdcb9921.png)


# MariaDB installation from repository (if normal installation not working)

#### Add the MariaDB GPK Key
```linux
sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xF1656F24C74CD1D8
```

#### Import key here
```linux
sudo add-apt-repository 'deb [arch=amd64,arm64,ppc64el] http://mirrors.accretive-networks.net/mariadb/repo/10.3/ubuntu bionic main'
```

#### Linux Update
```
sudo apt update && sudo apt upgrade -y
```

#### Add the additionals packets
```
sudo apt-get install software-properties-common -y
```


#### install mariadb server
```linux
sudo apt install mariadb-server -y
```

#### Check the mariadb status
```linux
sudo systemctl status mariadb
```

#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154024692-03df9fe3-113e-4047-a71b-f9e89c8dbf78.png)

#### Check the mysql version

```linux 
mysql -v
```
#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154025047-df08e9ab-4016-4bf6-8e6e-5e16fdcb9921.png)


#### A short tutorial on the base and management!

#### Securing MariaDB
```linux
sudo mysql_secure_installation
```

#### Connect to MariaDB
```linux
mysql -u root -p
```

#### Create a new MySQL database
```mysql
CREATE DATABASE database_name;
```

#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154026507-28ee9f22-5c7b-47bd-bd84-e8ca2f0e3211.png)


#### list all MySQL Databases
```mysql
SHOW DATABASES;
```

#### Delete MySQL database
```mysql
DROP DATABASE database_name;
```
#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154026697-72794abb-4fdf-47da-8684-0d5080d023cd.png)

#### Creating new user
```mysql
CREATE USER 'database_user'@'127.0.0.1' IDENTIFIED BY 'password_here';
```
#### Output The output should look like this!
![image](https://user-images.githubusercontent.com/65517973/154026825-bfc16d2f-89cf-4ced-b6ec-c4dfeb216e1f.png)

#### List of all MySQL users
```mysql
SELECT user, host FROM mysql.user;
```

#### Delete MySQL user
```mysql
DROP USER 'database_user@'localhost';
```

