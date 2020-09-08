# Wordpress
Bash script that uses Docker to setup and manage a local WordPress installation.

## Prerequisites

### Install Docker

First, you need to install Docker and start it. It's really easy. Just follow the instructions for your OS:

*   [Mac](https://docs.docker.com/docker-for-mac/install/)
*   [Windows](https://docs.docker.com/docker-for-windows/install/)
*   [Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
*   [Fedora](https://docs.docker.com/engine/install/fedora/)
*   [Other](https://docs.docker.com/engine/install/)

### Install this script

Download [the script](https://github.com/Kntnt/wordpress/blob/master/wordpress), put in your path and make it executable.

## Using 

### Initializing

To setup a project directory, create an empty directory, enter into it, and execute following command:

```bash
wordpress init
```

This creates the file `docker-compose.yml` in the directory. It is necessary for the script to work.

## Start

To start WordPress, enter the project directory, and execute following command:

```bash
wordpress up
```

The WordPress site is up and running within a minute or so after the command has finished.

### Logging

To see what's happening, enter the project directory, and execute following command:

```bash
wordpress logs
```

Leave the log view by pressing `CTRL C`.

## Stop

To stop WordPress, enter the project directory, and execute following command:

```bash
wordpress down
```

### Reset

To stop WordPress, free emory and remove all files, enter the project directory, and execute following command:

```bash
wordpress reset
```

## Accessing your Wordpress and database

### WordPress

To see your WordPress site, point your browser to http://localhost and be amazed.

### Database

Yo have [phpMyAdmin](https://docs.phpmyadmin.net/en/latest/) available at http://localhost:8080/. Use `root` and `password` as username and password, respectively.
