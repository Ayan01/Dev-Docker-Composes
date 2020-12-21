# Dev Docker Composes
A collection of Docker Compose files for quickly setting up dev environment. The collection contains some of the most popular services used in development of modern services and applications. 
- The compose files takes care of the hassle of downloading and then going through the process to setting up and configuring the services/clients on local dev machines by offloading it to Docker.
- All services are paired up with their monitoring/visualization/interaction clients (if available) for better control and dev experience.
- A single command to bring up the services along with the client and ready for development use.

## Setup

- Simply clone or download the repository or the docker-compose of your choice.
- Make sure docker is up and running.
- Open a terminal and navigate inside the directory of the docker-compose you want to setup.
- Run `docker-compose up -d`

That's it, your images will be downloaded and deployed in containers ready to use.

## The Collection

- Couchbase (2 Node Cluster)
- HazelCast (2 Node Cluster) with Hazelcast Management
- MongoDB with Mongo Express **\***
- Elasticsearch (Single Node) with Kibana
- Elasticsearch (2 Node Cluster) with Kibana
- MySQL with Adminer
- PostgreSQL with pgAdmin **\***
- Redis (Single Node) with RedisInsight

[**\*** The server(s)/client(s) requires some credentials to be set in the environment variables to start up or setup the service properly. By default, the bare minimum required credentials are set in the environment variables. If you choose to change the credentials, please go through the **docker-compose.yaml** file and update the corresponding environment variables before you do `docker-compose up -d`.]