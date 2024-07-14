Client gateway
The gateway is the communication point between our clients and our services. It is responsible for receiving requests, sending them to the corresponding services and returning the response to the client.

developer
Clone the repository
installed dependencies
Create an .env file based on the env.template
run nats : docker run -d --name nats-main -p 4222:4222 -p 6222:6222 -p 8222:8222 nats
Have the microservices that are going to be consumed up and running
Start project with npm run start:dev

#PROD

 docker build -f dockerfile.prod -t client-gateway .
