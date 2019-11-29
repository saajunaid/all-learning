* [Database Ranking and Descriptions](https://db-engines.com/en/ranking) 
* [Database Schemas and Models Samples](http://www.databaseanswers.org/data_models/)
# Mysql 
* [Official Mysql Docker hub location and documentation](https://hub.docker.com/_/mysql/)

* Download mysql from docker hub and map port 3306 on local machine to port 3306 of Docker Container with **myqsl-test** as the name of the Container and **test** as the password of Mysql, refer to websites below and the command is below.
* https://developer.ibm.com/tutorials/docker-dev-db/
* https://medium.com/@guilhermecoradini/how-to-crete-a-mysql-docker-container-exposing-it-to-mysql-workbench-3f78ea4a5455
  > docker run -p 3306:3306 --name mysql-test -e MYSQL_ROOT_PASSWORD=test -d mysql
* Connect to Mysql DB using mysql cli on local machine. You need to have mysql client istalled on your local machine for this to work.
  > junaid@linux-mint:~$ mysql -P 3306 --protocol=tcp -u root -p
* Or you can connect using mysql client running in another container as described in official Mysql Dockerhub documentation.
  > $ docker run -it --network some-network --rm mysql mysql -hsome-mysql -uexample-user -p
  
* Mysql cli Commands
  > https://gist.github.com/hofmannsven/9164408

#### Backup & Export

* Create Backup of the Database in the mysql container onto local machine
  > junaid@linux-mint:~/DataDumps$ docker exec mysql-test sh -c 'exec mysqldump customer -uroot -p"$MYSQL_ROOT_PASSWORD"' > /home/junaid/DataDumps/cust_data.sql
  
* [Export database to CSV](https://forums.aws.amazon.com/thread.jspa?threadID=41443)
