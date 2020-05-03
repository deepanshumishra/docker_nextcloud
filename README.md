# docker_nextclod

these days i am working on docker (containerization tool)
and i came across the idea of launching a cloud server used to share and collaborate on documents, send and receive email, manage calendar and have video chats.

nextcloud can be thinked as an opensource alternative for google drive,

i've used docker image nextcloud (https://hub.docker.com/_/nextcloud) and external database mariadb, docker image of mariadb can be downloaded from (https://hub.docker.com/_/mariadb)

we can use mysql docker image too but here i've used mariadb due to some reasons:
1. MariaDB shows an improved speed when compared to MySQL.
2. With the Memory storage engine of MariaDB, an INSERT statement can be completed 24% faster than in the standard MySQL.


> as nextcloud is the opensource and free to use we can easily launch this on our private server.

**prerequisites to launch above setup:**
i am using redhat8 as the host but you can use any linux distro
1. install docker-ce
> installation guide for docker is here https://docs.docker.com/engine/install/
2. install docker-compose
> installation guide for docker-compose is here https://docs.docker.com/compose/install/
 this setup can be done just in one click by running below file in host
 make a directory in "/"
 `mkdir MyCompose`
 `cd MyCompose`
 and now paste the above file into this directory

after saving above file just type `docker-compose up -d`
to run the whole setup in one go
now to terminate the setup type command: `docker-compose stop`
as we have used persistent storage our data will be back once we launch the containers again with the help of docker-compose file provide above.

if you face any problem in setting up the whole infrastructure ping me at deepanshusuper16@gmail.com
i'll be very happy to help you :)


