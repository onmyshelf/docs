# OnMyShelf Administration Guide

**Note**: This documentation is not complete yet. More to come!

## Introduction
As OnMyShelf is a web application, it is made for being installed on a web server that can be reached from Internet or a local network.

Nevertheless, you are free to install it on a local computer.

## Install with docker (recommended)
The easiest way to install OnMyShelf is to use the docker project.

### Requirements
You need to have [Git](https://git-scm.com/) installed on your machine.

If you can't use git, you can download and skip the following steps,
but it's not recommended, as you can miss some changes.

### Download the docker project
Clone the project:
```bash
git clone https://github.com/onmyshelf/docker.git onmyshelf-docker
cd onmyshelf-docker
```
**Note**: You can change the name `onmyshelf-docker` with anything you want.

If you don't use git, [download the git archive](https://github.com/onmyshelf/docker/archive/refs/heads/master.zip) and unzip it.

### Run install
Follow the [documentation here](https://github.com/onmyshelf/docker).

## Manual install
If you want to install OnMyShelf manually, which is far more complicated, you can follow these instructions:

### Requirements
- A MariaDB (>10.3) database (should also work with a recent MySQL server)
- A web server with rewrite module enabled, PHP 8.2+ and some PHP modules.

[Reading this file](https://github.com/onmyshelf/docker/blob/master/api/Dockerfile) will help you to find the needed PHP extensions.

### Configuration
Copy `config.default.php` to `config.php` then edit it.

### Initialize database
Go into the project folder then run:
```bash
php bin/oms install
```
