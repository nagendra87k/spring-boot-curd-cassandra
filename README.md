# spring-boot-curd-cassandra

#Docker Command:

docker run -d --name cassendra -p 9042:9042 cassandra:latest 

docker exec -it cassendra bash

cqlsh

CREATE KEYSPACE spring_boot_keyspace WITH replication = {'class':'SimpleStrategy', 'replication_factor' : 1};

CREATE TABLE user(id int PRIMARY KEY, name text, city text, state text);

INSERT INTO user(id,name,city,state) VALUES(1,'Nagendra Kumar','New Delhi','Delhi');

SELECT * FROM user;

exit
