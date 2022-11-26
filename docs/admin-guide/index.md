# OnMyShelf Administration Guide

**Note**: This documentation is not complete yet. More to come!

## Install with docker (the easiest way)
The easiest way to install OnMyShelf is to use the docker project.

### Requirements
You need to have [Git](https://git-scm.com/) installed on your machine.

If you don't want to, you can download and skip the following steps, but it's not recommended,
as you can miss some changes.

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

## Install manually (the hard way)
If you want to install OnMyShelf manually, follow these instructions:

### Requirements
- A MariaDB (>10.3) database (should also work with a recent MySQL server)
- A web server with rewrite module enabled, PHP 8.0+ and some PHP modules.

[Read this file](https://github.com/onmyshelf/docker/blob/master/api/Dockerfile) to help you find the needed PHP extensions.

### Configuration
Copy `config.default.php` to `config.php` then edit it.

### Initialize database
Go into the project folder then run:
```bash
php bin/oms install
```
