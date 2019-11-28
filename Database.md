* [Database Ranking and Descriptions](https://db-engines.com/en/ranking) 
# Mysql 
* Download mysql from docker hub and map port 3306 on local machine to port 3306 of Docker Container with **myqsl-test** as the name of the Container and **test** as the password of Mysql
* https://developer.ibm.com/tutorials/docker-dev-db/
* https://medium.com/@guilhermecoradini/how-to-crete-a-mysql-docker-container-exposing-it-to-mysql-workbench-3f78ea4a5455
  > docker run -p 3306:3306 --name mysql-test -e MYSQL_ROOT_PASSWORD=test -d mysql
* Connect to Mysql DB using mysql cli on local machine. You need to have mysql client istalled on your local machine for this to work. 
  > junaid@linux-mint:~$ mysql -P 3306 --protocol=tcp -u root -p

  
