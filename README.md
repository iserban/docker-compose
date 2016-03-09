# About this repo
This is a simple example of using Docker Compose. 


This will start a service called myfrontend (a simple web app deployed in a container running tomcat 7) and a service called service1 (app running in a container running tomcat 8) and link the 2 together.

----
## Usage
To start up services just run:

`docker-compose up`

To see the containers running and find out the container names you can then run:

`docker ps`

To connect to the myfrontend service run:

`docker exec -it <NAME_MYFRONTEND_CONTAINER> bash`

To test connectivity to service1 run:

`curl service1:8080/sample/`
