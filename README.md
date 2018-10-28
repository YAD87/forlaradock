1) Add to /etc/hosts
127.0.0.1 project-x.test

2) cd laradock folder and launch

docker-compose up -d nginx php-fpm mysql

3) check containers with 

docker ps


4) go to application container with
docker-compose exec --user=laradock workspace bash

5)Execute
 compose install

npm install

6) Go to browser by adress project-x.test


7) For connect to mysql db need go to mysql container
docker-compose exec mysql bash

and launch

mysql -u root -p

password root

and launch in mysql
grant all privileges on *.* to dev@localhost identified by 'develop1'
exit and try connect by dev user

mysql -u dev -p

password develop1

Created empty db for ap name db1
 


