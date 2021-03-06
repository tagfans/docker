# TagFans on Docker

Docker for Tagfans development.

## Installation

Please install [docker engine](https://docs.docker.com/engine/installation/) and [docker-compose](https://docs.docker.com/compose/install/) command first.

## Usage

Download source into your project.

```bash
$ cd  your_project_path
$ git clone https://github.com/tagfans/docker.git
$ cd docker
```

### Import MySQL Data

Open your terminal and execute the following command.

```bash
$ mysql -h 127.0.0.1 -u tagfans -p tagfans < db.sql
```

default password is `tagfans`.

### Start container

Start all application containers (Node, Mysql and Redis)

```bash
$ docker-compose up -d
```

### Stop container

Stop all application containers

```bash
$ docker-compose stop
```

### Remove container

Remove all application containers

```bash
$ docker-compose down
```
