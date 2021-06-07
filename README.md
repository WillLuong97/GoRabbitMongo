# GoRabbitMongo

GoRabbitMongo is a client microservies application with the sole purpose to write messages retrieved from a RabbitMQ cconsumer and store them into a Mongodb collection. This project is one of the many microservices to support the growing need of decoupling the architecture of Toodle. 

The key part of GoRabbitMongo is using RabbitMQ running on its own docker image as a way to store data from the client while waiting on the consumer. This way, if some backend services had to be taken down, the unprocessed data will
be stored temporarily on the RabbitMQ queue until the service is back online and continue the process. 

 

