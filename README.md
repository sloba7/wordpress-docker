# Docker Compose Setup for WordPress and MySQL

This Docker Compose setup allows you to quickly spin a WordPress application along with a MySQL database and a PHPMyAdmin instance for database management.

## Prerequisites

Before you get started, ensure that you have the following prerequisites installed on your system:


- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Usage

### 1. Clone this repository to your local machine.

```
git clone https://github.com/sloba7/wordpress-docker.git
cd wordpress-docker
```

### 2. Extract files from the site.zip



### 3. Run the Docker command to start the services:

```
docker-compose up -d
```

This command will start the MySQL database, WordPress, and PHPMyAdmin containers in the background.



### 4. Access the WordPress and PHPMyAdmin

PHPMyAdmin : http://localhost:8011

Wordpress : http://localhost:8001

Credentials are: 

- username: admin
- password: admin


## Data Presistence
 Data for the WordPress application and MySQL database is persisted in name volumes, so you won't lose your data even if you stop or remove the containers.
 - WordPress is stored in the wordpress volume.
 - MySQL data is stored in the database volume.


 ## Stop and Cleanup
  To stop the services and remove the containers, run:
```
docker-compose down
```
This sorts and removes the containers, but it won't delete the named volumes, preserving your data.
