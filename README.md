#  WordPress Docker Compose


## Installation

Open a terminal and `cd` to the folder in which `docker-compose.yml` is saved and run:

```
docker-compose up
```
## Usage

### Starting containers

You can start the containers with the `up` command in daemon mode (by adding `-d` as an argument) or by using the `start` command:

```
docker-compose start
```

### Stopping containers

```
docker-compose stop
```

### Removing containers

To stop and remove all the containers use the`down` command:

```
docker-compose down
```

Use `-v` if you need to remove the database volume which is used to persist the database:

```
  docker-compose down -v
```


### Creating database dumps

```
  ./export.sh
```


### install xdebug

insert in container wp

```
docker exec -it IDCONTAINER bash
```

```
pecl install -f xdebug-2.6.1

```
If has phpstorm you can to add config/php.conf.ini	

```
  #Example
  zend_extension="/usr/local/lib/php/extensions/no-debug-non-zts-20170718/xdebug.so" #file so
  xdebug.remote_enable=1
  xdebug.remote_host="IP"
  xdebug.idekey="PHPSTORM"
```


