# Wordpress MySQL Docker :whale2:

Code to fast setup a wordpress server with mysql database through docker.


## Dependencies

To run this project you will need Docker and docker-compose install
on you system, please check [here](https://docs.docker.com/compose/install/) to install both.


## Setup

You must before execute setup the root password for your database, open your docker-compose.yaml
and replace the `<password>` entries with your own password.


## Create webserver and database

To create and start your server run this command inside the project root folder:
```bash
docker-compose up
```

If some information telling you `permission denied` probably you have to run `sudo docker-compose up` or go through this [step](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user) to manage docker as non-root user.

If you desires to run this server on background add `-d` flag to docker-compose command:

```bash
docker-compose up -d
```

#### Start

```bash
docker-compose start
```

*Note*: if you run `docker-compose up` after you had initialized your webserver the docker compose will overwrite all data, therefore allways run `docker-compose start` if the webserver were created.

#### Stop

Just stop the containers:

```bash
docker-compose stop
```

#### Remove

This command will stop and delete all containers managed by this `docker-compose.yaml` file:

```bash
docker-compose rm
```


# Thanks

I will appreciate a lot if you suggest some improvement, please fork this project and request some pull of improvement :wink:
